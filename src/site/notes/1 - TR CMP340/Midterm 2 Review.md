---
{"dg-publish":true,"permalink":"/1-tr-cmp-340/midterm-2-review/"}
---

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
