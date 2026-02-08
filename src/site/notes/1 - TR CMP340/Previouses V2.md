---
{"dg-publish":true,"permalink":"/1-tr-cmp-340/previouses-v2/"}
---

## Table of Contents

- [[#September 16, 2025]]
- [[#September 30, 2025 — First Exam (Session #1)]]
- [[#September 30, 2025 — First Exam (Session #2)]]
- [[#October 20, 2025]]
- [[#October 21, 2025]]
- [[#November 24, 2025 (Quiz 3 — Source Vertex = 2)]]
- [[#November 24, 2025 (Quiz 3 — Source Vertex = 1)]]
- [[#Final Exam]]

---

#### September 16, 2025

**Given the following recursive function. Answer the following questions.**

```c
bool f(int i, int A[], int n) {
    if (i == n) return true;

    if (A[i] == A[i+1]) {
        return false;
    }

    return f(i + 1, A, n);
}
```

a. Write the initial call to this function.  
b. Show the execution (in detail) of this function when the input array is: 7, 12, 18.  
c. What is the controlling variable for this function?  
d. Explain the time complexity of the function in the worst and best cases.  
e. Explain the space complexity of the function in the worst and best cases.

---

#### September 30, 2025 — First Exam (Session #1)

**Q1.** (8 points) Show the execution of the algorithm on the array **A [7,3,9,2]** with **n=4**; track all variables, including the array. Calculate the running time using the sum operator (sigma).

```c
for (int i = n - 1; i >= 1; i--) {
    for (int j = 0; j < i; j++) {
        if (A[j + 1] < A[j]) {
            int x = A[j];
            A[j] = A[j + 1];
            A[j + 1] = x;
        }
    }
}
```

**Q2.** (7 points) Show the execution of the algorithm with pattern **[s, f]** and text **[s,g,s,s,f]**. Calculate the running time using the sum operator (sigma) in the worst-case and best-case scenarios, assuming the size of the pattern is **m**, while the size of the text is **n**.

```c
for (int i = 0; i < text.size() - pattern.size() + 1; i++) {
    bool found = true;
    for (int j = 0; j < pattern.size(); j++) {
        if (pattern[j] != text[i + j]) {
            found = false;
            break;
        }
    }
    if (found) return 1;
}
return 0;
```

**Q3.** (10 points) Show the execution of the algorithm, starting with the initial call, **f(4)**; track the call tree, local variables in each call, output displayed in each call, and the return value from each call. Calculate the running time and space using the complexity table.

```c
int f(int n) {
    if (n == 1) return 3;
    for (int i = 1; i <= n; i++)
        cout << i << " ";
    return f(n/2) + f(n/2);
}
```

---

#### September 30, 2025 — First Exam (Session #2)

**Q1.** (8 points) Show the execution of the algorithm (below) on the array **A [5,8,9,17,30,47,51]** with the initial call **BS(A,7,30)** (track all variables). Calculate the running time and space (stack size) using the complexity table.

```c
int BS(int A[], int n, int key) {
    int L = 0;
    int R = n - 1;
    while (L <= R) {
        int m = (L + R) / 2;
        if (A[m] < key)
            L = m + 1;
        else if (A[m] > key)
            R = m - 1;
        else return m;
    }
    return -1;
}
```

**Q2.** (8 points) Show the execution of the algorithm where **A [8,5,7,2]**; track all variables, including the array. Calculate the time in the best-case scenario using the sum operator (Sigma).

```c
for (int i = 1; i < n; i++) {
    int v = A[i]; int j;
    for (j = i - 1; j >= 0; j--) {
        if (v > A[j])
            break;
        A[j + 1] = A[j];
    }
    A[j + 1] = v;
}
```

**Q3.** (9 points) Demonstrate the execution of the following algorithm, where the initial call is **Func(3)** (track the call tree specifying in each call the value of n, and the return value). Illustrate the time and space complexity class of the algorithm using the complexity table method.

```c
int Func(int n) {
    if (n == 1) return 1;
    for (int i = 1; i <= 4; i++)
        cout << n << " ";
    return Func(n - 1) + Func(n - 1) + Func(n - 1);
}
```

---

#### October 20, 2025

**Q0.** **Apply Heapify(A,4,0) (defined below) to the array A [3,9,2,6] and respond to the following.** In a tree view, show all calls made for both **Heapify** and **siftdown**. In each call, show the changes of the local parameters (**i, left, and right**) and the swaps done on the array.

```cpp
void siftdown(int A[], int n, int i) {
    if (i >= n) return;
    int left = 2 * i + 1;
    int right = 2 * i + 2;
    if (left < n && A[left] >= A[i] && (right >= n || (right < n && A[left] >= A[right]))) {
        int x = A[i];
        A[i] = A[left];
        A[left] = x;
        siftdown(A, n, left);
    }
    else if (right < n && A[right] >= A[i] && A[right] >= A[left]) {
        int x = A[i];
        A[i] = A[right];
        A[right] = x;
        siftdown(A, n, right);
    }
}

void Heapify(int A[], int n, int i) {
    if (i >= n) return;
    int left = 2 * i + 1;
    int right = 2 * i + 2;
    Heapify(A, n, left);
    Heapify(A, n, right);
    if (left < n && A[left] >= A[i] && (right >= n || (right < n && A[left] >= A[right]))) {
        int x = A[i];
        A[i] = A[left];
        A[left] = x;
        siftdown(A, n, left);
    }
    else if (right < n && A[right] >= A[i] && A[right] >= A[left]) {
        int x = A[i];
        A[i] = A[right];
        A[right] = x;
        siftdown(A, n, right);
    }
}
```

**Q1.** Show the execution of the algorithm (below) on the array **A [8,2,6,3]** with size **n=4**, track all variables, including the array. Calculate the time complexity of the algorithm using the sum operator (**sigma**).

```cpp
for (int i = 0; i < n; i++) {
    for (int j = i + 1; j < n; j++) {
        if (A[j] < A[i]) {
            int x = A[i];
            A[i] = A[j];
            A[j] = x;
        }
    }
}
```

**Q2.** Track all variables in the execution of the algorithm on the list **[6,5,5,7]** with size **n=4**. Calculate the time using the sum operator (**sigma**). What is the impact on correctness & running time if we change the start value of **j** to **n-1**?

```cpp
int mode = list[n - 1], freq = 1;
for (int i = n - 1; i > 0; i--) {
    int m = list[i], f = 1;
    for (int j = i - 1; j >= 0; j--) {
        if (m == list[j]) f++;
    }
    if (f > freq) {
        mode = m; freq = f;
    }
}
```

**Q3.** Demonstrate the execution of the following algorithm, where the initial call is **Func(8)**; track the calls, the local variables of each call, and show the returned value from each call. Prove the time and space complexity class of the algorithm using the complexity table method.

```cpp
int Func(int n) {
    if (n == 1) return 2;
    for (int i = 1; i <= n/2; i++)
        cout << n << " ";
    return Func(n/2);
}
```

---

#### October 21, 2025

Apply the following quicksort algorithm to the array **A [7,4,0,3]** and respond to the following requirements. **What is the initial call to quicksort?** Show all calls to quicksort as a tree. Also, show the changes in local parameters for each call. Likewise, show the swaps in the array.

```c
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
        quicksort(p + 1, h, A);
        quicksort(l, p, A);
    }
}
```

**Q1.** Show the execution of Breadth First Search (given below) on the input graph. Show the changes in all variables, including the entries for all structures. Start tracking the changes within the highlighted segment. **What changes to the program below are required to process disconnected graphs?**

![imagep-1.png|400](/img/user/1%20-%20TR%20CMP340/img/imagep-1.png)

```c++
void bfs(vector<vector<int>> &graph, vector<int>& visited, vector<int>& queue) {
    while (!queue.empty()) {
        int i = queue[0];
        queue.erase(queue.begin());
        cout << "visited: " << i << endl;
        for (int j = 0; j < visited.size(); j++) {
            if (graph[i][j] == 1 && visited[j] == 0) {
                visited[j] = 1;
                queue.push_back(j);
            }
        }
    }
}

int main() {
    int n, m; // n vertices with m connections
    cout << "enter number of vertices: "; cin >> n;
    cout << "enter number of connections: "; cin >> m;
    vector<vector<int>> graph(n, vector<int>(n));
    vector<int> visited(n);
    vector<int> queue;
    for (int k = 0; k < m; k++) {
        cout << "enter connection (source target): ";
        int u, v; cin >> u >> v;
        graph[u][v] = graph[v][u] = 1;
    }

    for (int i = 0; i < n; i++) { visited[i] = 0; }
    queue.push_back(0);
    visited[0] = 1;
    bfs(graph, visited, queue);
}
```

**Q2.** Show the execution of quicksort (given below) on the array **A [4,6,3,7]**. Show all function calls, including the first call to "quicksort", the values of the functions' parameters, the changes in the variables, and the changes in the array.

```c
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
        quicksort(p + 1, h, A);
        quicksort(l, p, A);
    }
}
```

**Q3.** Show the execution of the transitive closure algorithm (given below) on the graph. Show all calls to dfs, the changes in the variables, including all structures. Start tracking the changes within the highlighted segment.

![imagep-2.png|400](/img/user/1%20-%20TR%20CMP340/img/imagep-2.png)

```c++
void dfs(int start, int i, vector<vector<int>> &graph, vector<int>& visited) {
    visited[i] = 1;
    for (int j = 0; j < visited.size(); j++) {
        if (graph[i][j] == 1) {
            graph[start][j] = 1;
            if (visited[j] == 0) dfs(start, j, graph, visited);
        }
    }
}

int main() {
    int n, m; // n vertices with m connections
    cout << "enter number of vertices: "; cin >> n;
    cout << "enter number of connections: "; cin >> m;
    vector<vector<int>> graph(n, vector<int>(n));
    vector<int> visited(n);
    for (int k = 0; k < m; k++) {
        cout << "enter connection " << k << " (source target): ";
        int u, v; cin >> u >> v;
        graph[u][v] = 1;
    }

    for (int i = 0; i < n; i++) {
        for (int i = 0; i < n; i++) visited[i] = 0;
        dfs(i, i, graph, visited);
    }

    cout << "The transitive closure of the graph is: " << endl;
    for (int i = 0; i < n; i++)
        for (int j = 0; j < n; j++)
            if (graph[i][j] == 1) cout << "edge: " << i << ", " << j << endl;
}
```

---

#### November 24, 2025 (Quiz 3 — Source Vertex = 2)

**Show the execution of the shortest path finding algorithm (given on the next page) on the following graph.** Start tracking the execution from the highlighted segment. Track all recursive calls, call parameters, local variables, and data structures. **The source vertex is 2.**

![imagep-4.png|400](/img/user/1%20-%20TR%20CMP340/img/imagep-4.png)

```cpp
int main() {
    int source, n, m;
    cout << "enter number of vertices: "; cin >> n;
    cout << "enter number of connections: "; cin >> m;
    cout << "enter the origin vertex: "; cin >> source;

    vector<vector<int>> graph(n, vector<int>(n));
    vector<int> visited(n), distance(n), finished(n), from(n);

    for (int i = 0; i < graph.size(); i++) {
        visited[i] = 0;
        finished[i] = 0;
        distance[i] = INT_MAX;
        from[i] = -1;
        for (int j = 0; j < graph[i].size(); j++) graph[i][j] = INT_MAX;
    }

    distance[source] = 0; finished[source] = 1; visited[source] = 1;

    for (int k = 0; k < m; k++) {
        cout << "enter directed connection " << k << " (vertex1 vertex2 weight): ";
        int u, v, w;
        cin >> u >> v >> w;
        graph[u][v] = w;
    }

    // highlighted segment:
    for (int i = 0; i < graph.size(); i++) {
        if (finished[i] == 0) {
            shortest(0, i, graph, visited, finished, distance, from);
            // 1 call runs in time O(n^2), but since repeated n times -> O(n^3)
            for (int &x : visited) x = 0;
        }
    }
}

void shortest(int C, int i,
              vector<vector<int>>& graph,
              vector<int>& visited,
              vector<int>& finished,
              vector<int>& distance,
              vector<int>& from) {

    visited[i] = 1;
    bool f = true;

    for (int j = 0; j < graph.size(); j++) {
        if (graph[j][i] < INT_MAX) {

            if (finished[j] == 1) {
                if (distance[j] + graph[j][i] < distance[i]) {
                    distance[i] = distance[j] + graph[j][i];
                    from[i] = j;
                }
            }
            else if (visited[j] == 0) {
                shortest(C + graph[j][i], j, graph, visited, finished, distance, from);
                if (distance[j] + graph[j][i] < distance[i]) {
                    distance[i] = distance[j] + graph[j][i];
                    from[i] = j;
                }
            }
            else {
                f = false;
                if (C + graph[j][i] < 0) {
                    cout << "neg cycle cost: " << (C + graph[j][i]) << endl;
                    exit(0);
                }
            }
        }
    }

    if (f) finished[i] = 1;
}
```

---

#### November 24, 2025 (Quiz 3 — Source Vertex = 1)

**Show the execution of the shortest path finding algorithm (given on the next page) on the following graph.** Start tracking the execution from the highlighted segment. Track all recursive calls, call parameters, local variables, and data structures. **The source vertex is 1.**

![imagep-3.png|400](/img/user/1%20-%20TR%20CMP340/img/imagep-3.png)

_(Same algorithm code as the source=2 variant above.)_

---

#### Final Exam

**Q1.** Calculate the time and space complexity of the following program using the complexity table.

```cpp
void g(int n) {
    if (n == 1) return;
    for (int i = 1; i <= n; i++) {
        for (int j = 1; j <= n; j++)
            i + j;
    }
    g(n - 1); g(n - 1); return;
}
int main() { int n; cin >> n; g(n); }
```

**Q2.** Fill in the tables (on the next page) with the progress of recursive calls (and their arguments & returns), the values of local variables, and the data structures' content during the execution of the following minimum_spanning_tree finding program. Tracking the execution of the sort function is not required.

```cpp
struct edge { int x, y, cost; };

void sort(vector<struct edge>& edges) {
    for (int i = 0; i < edges.size(); i++)
        for (int j = i + 1; j < edges.size(); j++)
            if (edges[j].cost < edges[i].cost) {
                edge e = edges[j]; edges[j] = edges[i]; edges[i] = e;
            }
}

bool cycle(int from, int i, vector<vector<int>>& graph, vector<int>& visited) {
    visited[i] = 1;
    for (int j = 0; j < graph.size(); j++) {
        if (j != from && (graph[i][j] == -1 || graph[j][i] == -1)) {
            if (visited[j]) return true;
            else if (cycle(i, j, graph, visited)) return true;
        }
    }
    return false;
}

void kruskal(vector<vector<int>>& graph, vector<edge> edges) {
    int i = 1; int j = 0;
    while (i < graph.size()) {
        vector<int> visited(graph.size());
        for (int& x : visited) x = 0;
        graph[edges[j].x][edges[j].y] = -1;
        if (!cycle(-1, edges[j].x, graph, visited))  i++;
        else graph[edges[j].x][edges[j].y] = 0;
        j++;
    }
}

int main() {
    int n, m; // n vertices with m connections
    cout << "enter number of vertices: ";       cin >> n;
    cout << "enter number of connections: ";     cin >> m;
    vector<vector<int>> graph(n, vector<int>(n));
    vector<int> visited(n);
    for (int i = 0; i < graph.size(); i++) {
        visited[i] = 0;
        for (int j = 0; j < graph[i].size(); j++)
            graph[i][j] = INT_MAX;
    }

    vector<struct edge> edges;
    for (int k = 0; k < m; k++) {
        cout << "enter connection " << k << " (source target weight): ";
        int u, v, w;
        cin >> u >> v >> w;
        graph[u][v] = w;
        struct edge e = { u, v, w };
        edges.push_back(e);
    }

    sort(edges);
    kruskal(graph, edges);
    for (int i = 0; i < graph.size(); i++)
        for (int j = 0; j < graph.size(); j++)
            if (graph[i][j] == -1)
                cout << "vertex " << i << " is connected with " << j << endl;
}
```

_(See graph below — 5 vertices (0–4) with weighted undirected edges, and blank tables for graph matrix, visited matrix, edges matrix, and call tracking.)_

![imagep-5.png|400](/img/user/1%20-%20TR%20CMP340/img/imagep-5.png)

**Q3.** Fill in the tables (on the next page) with the progress of recursive calls (and their arguments & returns), the local variables, and the arrays during the execution of the following program on the flow network on the next page. **Source=0, terminal=4.**

```cpp
struct edge { int capacity; int flow; };
int source, terminal, n, m;
vector<vector<edge>> g;
vector<int> visited;
vector<int> surplus;

void reduce(int i) {
    visited[i] = 1;
    for (int j = 0; j < n; j++) {
        if (surplus[i] == 0) return;
        if (visited[j] == 0 && g[j][i].flow > 0) {
            int t = surplus[j];
            if (surplus[i] >= g[j][i].flow) {
                surplus[i] -= g[j][i].flow;
                surplus[j] += g[j][i].flow; g[j][i].flow = 0;
            }
            else {
                g[j][i].flow -= surplus[i];
                surplus[j] += surplus[i]; surplus[i] = 0;
            }
            if (j != source && surplus[j] > 0) {
                reduce(j);
                if (surplus[j] > t) {
                    g[j][i].flow += surplus[j] - t;
                    surplus[i] += surplus[j] - t; surplus[j] = t;
                }
            }
        }
    }
}

void balance(int i, bool avoidTerm) {
    visited[i] = 1;
    for (int j = 0; j < n; j++) {
        if (surplus[i] >= 0) return;
        if (j == terminal && avoidTerm) continue;
        if (j == terminal)
            g[i][j].flow += surplus[i]; surplus[j] += surplus[i];
            surplus[i] = 0;      return;
        if (visited[j] == 0 && g[i][j].flow > 0 && surplus[j] > 0 && j != terminal) {
            if (surplus[j] > g[i][j].flow) {
                surplus[j] -= g[i][j].flow;
                surplus[i] += g[i][j].flow; g[i][j].flow = 0;
            }
            else {
                g[i][j].flow -= surplus[j];
                surplus[i] += surplus[j]; surplus[j] = 0;
            }
            if (surplus[i] >= 0) return;
        }
        if (visited[j] == 0 && g[i][j].flow > 0) {
            int t = surplus[j];
            if (abs(surplus[i]) >= g[i][j].flow) {
                surplus[i] += g[i][j].flow;
                surplus[j] -= g[i][j].flow; g[i][j].flow = 0;
            }
            else {
                g[i][j].flow += surplus[i];
                surplus[j] += surplus[i]; surplus[i] = 0;
            }
            if (surplus[j] < 0) {
                balance(j, avoidTerm);
                if (surplus[j] < t) {
                    g[i][j].flow -= surplus[j] - t;
                    surplus[i] += surplus[j] - t; surplus[j] = t;
                }
            }
        }
    }
}

int main() {
    cout << "enter number of vertices: ";   cin >> n;
    cout << "enter number of connections: "; cin >> m;
    g = vector<vector<edge>>(n, vector<edge>(n));
    visited = vector<int>(n); surplus = vector<int>(n);
    for (int k = 0; k < m; k++) {
        cout << "enter directed connection " << k << " (source target capacity): ";
        int u, v, c;
        cin >> u >> v >> c;
        g[u][v] = { c, c };
        surplus[u] -= c;
        surplus[v] += c;
    }
    cout << "specify the source vertex: "; cin >> source;
    cout << "specify the terminal: ";      cin >> terminal;
    surplus[source] = 0;

    // highlighted segment 1:
    for (int i = 0; i < n; i++) {
        for (int k = 0; k < n; k++) visited[k] = 0;
        if (surplus[i] < 0) {
            balance(i, true);
        }
    }
    // highlighted segment 2:
    for (int i = 0; i < n; i++) {
        for (int k = 0; k < n; k++) visited[k] = 0;
        if (surplus[i] < 0) {
            balance(i, false);
        }
    }
    // highlighted segment 3:
    for (int i = 0; i < n; i++) {
        for (int k = 0; k < n; k++) visited[k] = 0;
        if (i != source && i != terminal && surplus[i] > 0) {
            reduce(i);
        }
    }

    for (int i = 0; i < n; i++) {
        cout << "surplus " << i << ": " << surplus[i] << endl;
        for (int j = 0; j < n; j++) {
            if (g[i][j].flow > 0) {
                cout << "\nFlow from " << i << " to " << j << ": " << g[i][j].flow;
            }
        }
    }
}
```

_(See flow network below — 5 vertices (0–4) with directed capacitated edges. Graph matrix, visited matrix, surplus matrix, and call-tracking table provided as blanks.)_

![imagep-6.png|400](/img/user/1%20-%20TR%20CMP340/img/imagep-6.png)

**balance() and reduce() code reference:**

![imagep-7.png|400](/img/user/1%20-%20TR%20CMP340/img/imagep-7.png)

**Q4.** Fill in the table with the progress of calls, their local variables during the execution of the following program running on the graph on the next page. Show the time and space complexity of the following program using the complexity table.

```cpp
vector<int> sol;

void max_ind_set(int v, vector<int>& X, vector<int>& degree,
                 vector<int>& status, vector<vector<int>>& graph) {
    vector<int> in;
    in.push_back(v); X.push_back(v);
    while (!in.empty()) {
        int i = in[in.size() - 1]; in.pop_back();
        for (int j = 0; j < graph.size(); j++) {
            if (graph[i][j] == 1 && status[j] == -1) {
                status[j] = 0;
                for (int k = 0; k < graph.size(); k++) {
                    if (graph[j][k] == 1 && status[k] == -1) {
                        degree[k]--;
                        if (degree[k] == 0) {
                            status[k] = 1;
                            in.push_back(k);
                            X.push_back(k);
                        }
                    }
                }
            }
        }
    }

    bool collectSol = true;
    for (int i = 0; i < graph.size(); i++) {
        if (status[i] == -1) {
            collectSol = false;
            status[i] = 1;
            max_ind_set(i, X, degree, status, graph);
            status[i] = 0;
        }
    }

    if (collectSol) if (sol.size() == 0 || (X.size() > sol.size())) sol = X;
}

void main() {
    int n; cout << "enter number of vertices: ";     cin >> n;
    int m; cout << "enter number of connections: ";   cin >> m;
    vector<vector<int>> graph(n, vector<int>(n));
    vector<int> status(n);
    vector<int> degree(n);

    for (int i = 0; i < graph.size(); i++) {
        status[i] = -1;
        degree[i] = 0;
    }
    for (int k = 0; k < m; k++) {
        cout << "enter undirected connection " << k << " (vertex1 vertex2): ";
        int u, v; cin >> u >> v;
        graph[u][v] = graph[v][u] = 1;
        degree[u]++; degree[v]++;
    }

    vector<int> X;
    for (int i = 0; i < graph.size(); i++) {
        status[i] = 1;
        max_ind_set(i, X, degree, status, graph);
        status[i] = 0;
    }

    cout << "The max ind set: " << endl;
    for (int k = 0; k < sol.size(); k++) cout << sol[k] << endl;
}
```

_(See graph below — 4 vertices (0–3) with undirected edges, and blank tables for X, visited, degree, status, and call tracking.)_

![imagep-8.png|400](/img/user/1%20-%20TR%20CMP340/img/imagep-8.png)

**Time and Space Complexity Analysis (3 marks)** _(Blank page for complexity analysis of Q4's algorithm.)_