---
{"dg-publish":true,"permalink":"/1-tr-cmp-340/midterm-2-review/"}
---

[[#W6 Quicksort, DFS, BFS]]
[[#W7 Advanced string matching, Hashing, Heapsort]]
[[#W8 Prim's Algorithm]]
[[#W9 Kruskal]]

# W6: Quicksort, DFS, BFS

### Quicksort
```cpp
int partition(int l, int h, int A[]) {
    int pivot = A[l]; int i = l - 1, j = h + 1;
    while (true) {
        do i = i + 1; while (A[i] < pivot);
        do j = j - 1; while (A[j] > pivot);
        if (i < j) {
            int k = A[i];
            A[i] = A[j];
            A[j] = k;
        }
        else return j;
    }
}

void quicksort(int l, int h, int A[]) {
    if (l < h) {
        int p = partition(l, h, A);
        quicksort(p+1, h, A);
        quicksort(l, p, A);
    }
}
```

Quicksort example
![image-146.png](/img/user/1%20-%20TR%20CMP340/img/image-146.png)

Quicksort time and space complexity
![image-147.png](/img/user/1%20-%20TR%20CMP340/img/image-147.png)

**Worst case vs best case: when does it happen?**
![image-154.png|570](/img/user/1%20-%20TR%20CMP340/img/image-154.png)

**Why is quicksort unstable?**
![image-155.png|547](/img/user/1%20-%20TR%20CMP340/img/image-155.png)


### DFS / BFS
Graph: node (vertices) connected by lines (edges)
![image-149.png|400x338](/img/user/1%20-%20TR%20CMP340/img/image-149.png)

For undirected graphs, you set both graph\[u]\[v] and graph\[v]\[u] to 1.
![image-153.png|400x387](/img/user/1%20-%20TR%20CMP340/img/image-153.png)

DFS vs BFS
![image-150.png|400x277](/img/user/1%20-%20TR%20CMP340/img/image-150.png)
BFS **marks visited AND enqueues** when it **discovers** a neighbor (not when it processes it). 

Both DFS and BFS have identical complexity tables.
![image-151.png|400x184](/img/user/1%20-%20TR%20CMP340/img/image-151.png)

**What handles disconnected graphs** (Graphs where some vertices have no path between them)**?**
`for` loop in main
```cpp
for (int i = 0; i < n; i++) {
    if (visited[i] == 0) {
        dfs(i, graph, visited);  // starts a new traversal from each unvisited node
    }
}
```
> Without it, nodes with no path from the start would never be visited

![image-152.png|400x222](/img/user/1%20-%20TR%20CMP340/img/image-152.png)
> So here 2->0 exists but 0->2 doesn't. Therefore, 0 is disconnected from rest. If you only run DFS from 0, you won't visit 1,2,3. That's why you iterate so next you start from 1, then 2 (if not visited from 1), etc.


**Format (what to show)?**
![image-156.png|400x89](/img/user/1%20-%20TR%20CMP340/img/image-156.png)

DFS
![image-159.png|625](/img/user/1%20-%20TR%20CMP340/img/image-159.png)
> [!info]- Alternative view
> ![image-157.png|400x303](/img/user/1%20-%20TR%20CMP340/img/image-157.png)

BFS
![image-158.png](/img/user/1%20-%20TR%20CMP340/img/image-158.png)

> [!abstract]- Codes
> **DFS:**
> ```cpp
> #include <iostream>
> #include <vector>
> using namespace std;
> 
> void dfs(int i, vector<vector<int>> graph, vector<int> &visited) {
>     visited[i] = 1;
>     cout << "visiting: " << i << endl;
>     for (int j = 0; j < visited.size(); j++) {
>         if (graph[i][j] == 1 && visited[j] == 0) {
>             dfs(j, graph, visited);
>         }
>     }
> }
> 
> int main() {
>     int n, m;
>     cout << "enter number of vertices: ";
>     cin >> n;
>     cout << "enter number of connections: ";
>     cin >> m;
>     vector<vector<int>> graph(n, vector<int>(n));
>     vector<int> visited(n);
>     for (int k = 0; k < m; k++) {
>         cout << "enter connection " << k << " (source target): ";
>         int u, v;
>         cin >> u >> v;
>         graph[u][v] = 1;
>     }
>     for (int i = 0; i < n; i++)
>         visited[i] = 0;
>     for (int i = 0; i < n; i++) {
>         if (visited[i] == 0) {
>             dfs(i, graph, visited);
>         }
>     }
> }
> ```
> 
> **BFS:**
> 
> ```cpp
> void bfs(vector<vector<int>> graph, vector<int>& visited, vector<int> &queue) {
>     while (!queue.empty()) {
>         int i = queue[0];
>         queue.erase(queue.begin());
>         cout << "visited: " << i << endl;
>         for (int j = 0; j < visited.size(); j++)
>             if (graph[i][j] == 1 && visited[j] == 0) {
>                 visited[j] = 1;
>                 queue.push_back(j);
>             }
>     }
> }
> 
> int main() {
>     int n, m;
>     cout << "enter number of vertices: "; cin >> n;
>     cout << "enter number of connections: "; cin >> m;
>     vector<vector<int>> graph(n, vector<int>(n));
>     vector<int> visited(n);
>     vector<int> queue;
>     for (int k = 0; k < m; k++) {
>         cout << "enter connection (source target): ";
>         int u, v; cin >> u >> v;
>         graph[u][v] = graph[v][u] = 1;
>     }
>     for (int i = 0; i < n; i++) { visited[i] = 0; }
>     for (int i = 0; i < n; i++) {
>         if (visited[i] == 0) {
>             queue.push_back(i);
>             visited[i] = 1;
>             bfs(graph, visited, queue);
>         }
>     }
> }
> ```
> 
> Note — DFS `main()` reads directed edges (`graph[u][v] = 1` only), BFS `main()` reads undirected (`graph[u][v] = graph[v][u] = 1`). That's how Dr. Nofal wrote them in the slides. The graph type depends on the problem, not the algorithm. Now trace both on the undirected graph.


![image-160.png|400x279](/img/user/1%20-%20TR%20CMP340/img/image-160.png)

# W7: Advanced string matching, Hashing, Heapsort 

### Advanced String Matching
The old brute-force pattern matching (from M1) slides the pattern across the text one position at a time and compares every character. Worst case: O(mn).

NEW METHOD: Instead of starting from the first character of the pattern, start from the least frequent character

**Why least?**
![image-161.png|400x244](/img/user/1%20-%20TR%20CMP340/img/image-161.png)
> old vs new "advanced" method


```cpp
// Phase 1: Build dictionary
/*
For each letter in the alphabet, store all positions where it appears in the text. This is just 26 vectors (one per letter), each holding index positions.
*/
vector<int> dictionary[26];
for (int i = 0; i < text.size(); i++)
    dictionary[text[i] - 'a'].push_back(i);

// Phase 2: Find least frequent char (anchor) in pattern
/*
Scan the pattern, check which pattern character has the fewest occurrences in the text. That's your anchor character.
*/
char least = pattern[0]; int position = 0;
int freq = dictionary[pattern[0] - 'a'].size();
for (int j = 1; j < pattern.size(); j++)
    if (freq > dictionary[pattern[j] - 'a'].size()) {
        least = pattern[j];
        freq = dictionary[pattern[j] - 'a'].size();
        position = j;
    }

// Phase 3: Search using the anchor
/*
For each position where the anchor appears in the text, check backwards (characters before the anchor) then forwards (characters after). If both match, you found it.
*/
for (int i = 0; i < dictionary[least - 'a'].size(); i++) {
    int index = dictionary[least - 'a'][i];
    int k = position - 1;
    bool found = true;
    // backward check
    for (int j = index - 1; j >= index - position; j--) {
        if (pattern[k--] != text[j]) {
            found = false; break;
        }
    }
    if (found) {
        int k = position + 1;
        // forward check
        for (int j = index + 1; j < index + pattern.size() - position; j++) {
            if (pattern[k++] != text[j]) {
                found = false; break;
            }
        }
        if (found) { cout << "found at " << index - position << endl; return 0; }
    }
}
cout << "not found" << endl;
```

Write down:
1. **Pattern + text with indices**
2. **26 slot Dictionary**
3. **Phase 2 table**
4. **Phase 3 table**

Example solving
![image-162.png](/img/user/1%20-%20TR%20CMP340/img/image-162.png)

Time & Space
![image-163.png|556](/img/user/1%20-%20TR%20CMP340/img/image-163.png)

### Hashing
![image-164.png|400x270](/img/user/1%20-%20TR%20CMP340/img/image-164.png)

For the exam:
- Compute h(k) = k mod m for each value
- Draw the chains
- Know the complexity (O(n/m) average, O(n) worst, O(1) best, O(m+n) space)

Example
![image-166.png|400x144](/img/user/1%20-%20TR%20CMP340/img/image-166.png)

### Heapsort
https://claude.ai/public/artifacts/2aa5d592-8a1f-408c-b5bb-468ab8326ec8

**Max-heap**
![image-15.png|400x324](/img/user/1%20-%20TR%20CMP340/img/image-15.png)
> **Parent** at `(i-1) / 2`

**Siftdown**
![image-16.png|400x252](/img/user/1%20-%20TR%20CMP340/img/image-16.png)

```cpp
void siftdown(int A[], int n, int i) {
    if (i >= n) return;
    int left = 2 * i + 1;
    int right = 2 * i + 2;
    if (left < n && A[left] >= A[i] && (right >= n || A[left] >= A[right])) {
        int x = A[i]; A[i] = A[left]; A[left] = x;
        siftdown(A, n, left);
    }
    else if (right < n && A[right] >= A[i] && A[right] >= A[left]) {
        int x = A[i]; A[i] = A[right]; A[right] = x;
        siftdown(A, n, right);
    }
}
```

For left
- Left child exists (`left < n`)
- Left child is ≥ parent (`A[left] >= A[i]`) — parent is too small
- Left child is the better swap — either there's no right child (`right >= n`) OR left ≥ right (`A[left] >= A[right]`)

> For right, same just with right child checks
> if neither triggers, do nothing (leaf or bigger than both children)

**Heapify**
bottoms-up

notice the code almost **identical** to siftdown, just with two recursive calls at the top:
```cpp
void Heapify(int A[], int n, int i) {
    if (i >= n) return;
    int left = 2 * i + 1;
    int right = 2 * i + 2;
    Heapify(A, n, left);       // ← fix left subtree first
    Heapify(A, n, right);      // ← fix right subtree second
    // then do exactly what siftdown does:
    if (left < n && A[left] >= A[i] && (right >= n || A[left] >= A[right])) {
        int x = A[i]; A[i] = A[left]; A[left] = x;
        siftdown(A, n, left);
    }
    else if (right < n && A[right] >= A[i] && A[right] >= A[left]) {
        int x = A[i]; A[i] = A[right]; A[right] = x;
        siftdown(A, n, right);
    }
}
```
> difference: 
> siftdown: Fix one node position
> heapify: Fix everything below me first, THEN fix me

Heapify once to build (*unsorted array → valid max-heap*), siftdown repeatedly to maintain

**main code**
```cpp
int main() {
    const int n = 5;
    int A[n] = {2, 5, 6, 8, 9};

    Heapify(A, n, 0);            // Stage 1: build max-heap

    for (int i = 0; i < n; i++) {    // Stage 2: sort
        int x = A[0];                // save the max
        A[0] = A[n - i - 1];        // move last element to root
        A[n - i - 1] = x;           // put max at the end
        siftdown(A, n - i - 1, 0);  // fix the heap (shrunk by 1)
    }
}
```
- **Swap** root (max) with the last unsorted element
- **Shrink** heap size by 1 (the swapped max is now in its final spot)
- **Siftdown** the new root to restore the heap

Make:
1. heapify and siftdown call tree
2. sort loop in main
![image-176.png|400x359](/img/user/1%20-%20TR%20CMP340/img/image-176.png)
![image-177.png|400x221](/img/user/1%20-%20TR%20CMP340/img/image-177.png)


**Siftdown time complexity** 
![image-167.png|400x193](/img/user/1%20-%20TR%20CMP340/img/image-167.png)
> Best case: O(1) if parent already bigger than children

![image-168.png|400x365](/img/user/1%20-%20TR%20CMP340/img/image-168.png)


# W8 Prim's Algorithm
![image-169.png|400x228](/img/user/1%20-%20TR%20CMP340/img/image-169.png)
- Input is always **connected, undirected, weighted** (symmetric matrix)
- For n vertices, the MST always has exactly n-1 edges
- Output is always **no cycles**

- `visited[i]` — is vertex i in the tree yet?
- `dist[i]` — cheapest known edge cost to reach vertex i
- `from[i]` — which vertex provides that cheapest edge?

![image-170.png|400x192](/img/user/1%20-%20TR%20CMP340/img/image-170.png)
1. **Mark current vertex visited**
2. **Scan all unvisited neighbors** — if the edge to them is cheaper than their current `dist`, update `dist` and `from`
3. **Pick the unvisited vertex with the smallest `dist`** — that's `min`
4. **Recurse on `min`**
5. **Stop when all vertices are visited** (`min` stays -1)

```cpp
void mst(int i, vector<vector<int>> &graph, vector<int>& visited,
         vector<int>& from, vector<int>& dist) {
    visited[i] = 1;
    int min = -1;
    for (int j = 0; j < graph.size(); j++) {
        if (visited[j] == 0) {
            if (dist[j] > graph[i][j]) {
                dist[j] = graph[i][j];
                from[j] = i;
            }
            if (min == -1) min = j;
            if (dist[min] > dist[j]) min = j;
        }
    }
    if (min != -1)
        mst(min, graph, visited, from, dist);
}
```

```cpp
int main() {
    int n, m;
    cin >> n;                    // number of vertices
    cin >> m;                    // number of edges

    vector<vector<int>> graph(n, vector<int>(n));
    vector<int> visited(n), from(n), dist(n);

    for (int i = 0; i < graph.size(); i++) {
        visited[i] = 0;         // nobody visited yet
        from[i] = -1;           // no connections yet
        dist[i] = INT_MAX;      // all distances = infinity
        for (int j = 0; j < graph[i].size(); j++)
            graph[i][j] = INT_MAX;  // no edges = infinity (not 0!)
    }
    for (int k = 0; k < m; k++) {
        int u, v, w;
        cin >> u >> v >> w;
        graph[u][v] = w;
        graph[v][u] = w;        // undirected = both directions
    }
    mst(0, graph, visited, from, dist);

    for (int i = 0; i < n; i++)
        if (from[i] != -1)      // skip the starting vertex
            cout << i << " connected with " << from[i] << endl;
}
```

> Time and Space complexity is EXACTLY like DFS 

![image-171.png|400x473](/img/user/1%20-%20TR%20CMP340/img/image-171.png)

# W9 Kruskal
Both Prim's and Kruskal's find the MST.
**Prim's:** Grows the tree from one vertex, always adding the cheapest edge to an unvisited neighbor

**Kruskal's:** Sorts ALL edges by cost, then adds them one by one (cheapest first), skipping any that would create a cycle

![image-172.png|400x234](/img/user/1%20-%20TR%20CMP340/img/image-172.png)

1. **Sort** all edges by cost (ascending)
2. **For each edge** (cheapest first): tentatively add it to the tree, then run DFS to check for cycles
3. If **no cycle** → keep it, increment edge count. If **cycle** → undo (remove it)
4. **Stop** when you have n-1 edges

**Data Structures**
```cpp
class vertex { //linked list node.
public:
    int label;           //neighbor's ID
    int cost = INT_MAX;  //weight
    vertex* next = NULL; //pointer to next neighbor
};

class adjList {
public:
    vertex* start = NULL; 
    void addAdjVer(int i, int c) { // add edge
        vertex* v = new vertex();
        v->label = i;
        v->cost = c;
        v->next = start;
        start = v;
    }
    void removeAdjVer() {
        vertex* v = start;
        start = start->next;
        delete v;
    }
};

class edge {
public:
    int x, y, cost;
};
```

**Sort**
```cpp
// it can be any sort. Here it is selection sort. You don't need to trace this — the exam says "tracking the execution of the sort function is not required."
void sort(vector<edge>& edges) {
    for (int i = 0; i < edges.size(); i++)
        for (int j = i + 1; j < edges.size(); j++)
            if (edges[j].cost < edges[i].cost) {
                edge e = edges[j];
                edges[j] = edges[i];
                edges[i] = e;
            }
}
```

**Kruskal**
```cpp
void kruskal(int n, vector<edge> &edges, vector<adjList> &tree) {
    int i = 1;                              // edges accepted so far
    int j = 0;                              // index into sorted edges
    while (i < n) {                         // need n-1 edges
        vector<bool> visited(n);
        // Step 1: tentatively add this edge (undirected)
        tree[edges[j].x].addAdjVer(edges[j].y, edges[j].cost);
        tree[edges[j].y].addAdjVer(edges[j].x, edges[j].cost);
        // Step 2: check for cycle
        bool cycle = false;
        for (int k = 0; k < n; k++) {
            if (!visited[k]) {
                if (check_cycle(-1, k, visited, tree)) {
                    cycle = true; break;
                }
            }
        }
        // Step 3: keep or undo
        if (!cycle)
            i++;                            // keep edge
        else {
            tree[edges[j].x].removeAdjVer();  // undo
            tree[edges[j].y].removeAdjVer();
        }
        j++;                                // next edge regardless
    }
}
```

**Cycle detection**
DFS on tree built so far.
```cpp
bool check_cycle(int from, int i, vector<bool>& visited, vector<adjList>& tree) {
    visited[i] = true;
    vertex* v = tree[i].start;
    while (v != NULL) {
        if (visited[v->label] && v->label != from) return true; //visited and not parent -> cycle found. return true.
        else if (!visited[v->label]) { //not visited recurse deeper
            if (check_cycle(i, v->label, visited, tree))
                return true;
        }
        v = v->next;
    }
    return false;
}
```

![image-173.png|400x277](/img/user/1%20-%20TR%20CMP340/img/image-173.png)
Why do we need to check for cycle?

**main()**
```cpp
int main() {
    int n;
    cin >> n;
    vector<vector<int>> graph(n, vector<int>(n));
    vector<edge> edges;
    for (int i = 0; i < n; i++) {
        for (int j = i + 1; j < n; j++) {
            int c; cin >> c;
            if (c == -1) c = INT_MAX;
            graph[i][j] = c;
            graph[j][i] = c;
            struct edge e = { i, j, c };
            edges.push_back(e);
        }
    }
    sort(edges);
    vector<adjList> tree(n);
    kruskal(n, edges, tree);
    vector<bool> visited(n);
    printTree(0, visited, tree);
}
```

- **Sort:** O(m²) with selection sort (or O(m log m) with heapsort)
- **Kruskal loop:** O(mn) — at most m iterations, each cycle check is O(n)
- **Total time:** O(mn + m²)
- **Total space:** O(m + n²) — graph matrix + edges list + visited + stack

![image-174.png|400x439](/img/user/1%20-%20TR%20CMP340/img/image-174.png)
![image-175.png|400x541](/img/user/1%20-%20TR%20CMP340/img/image-175.png)

