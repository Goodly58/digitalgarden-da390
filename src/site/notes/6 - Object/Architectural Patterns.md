---
{"dg-publish":true,"permalink":"/6-object/architectural-patterns/"}
---


### 🪜 Layered Pattern

> [!abstract]
> 
> - System divided into **layers**, each providing services to the one above.
>     
> - Promotes **modularity**, **reusability**, and **separation of concerns**.
>     
> - <span class="neon-highlight">We saw this in Operating Systems and Computer Networks</span>.
>     

![image-2.png|400](/img/user/6%20-%20Object/img/image-2.png)

---

### 🖥️ Client–Server Pattern

> [!note]
> 
> - **Client** requests services; **Server** provides them.
>     
> - Components can be on different machines (distributed).
>     

![image-1.png|400](/img/user/6%20-%20Object/img/image-1.png)

---

### 🧮 Pipe & Filter Pattern / Data flow systems

> [!example]
> 
> - Each **Filter** transforms data; **Pipes** pass it along.
>     
> - Used in **data-flow systems**, compilers, or stream processing.
>     


![image.png](/img/user/6%20-%20Object/img/image.png)

- DataSource
- DataSink
- Filter

![image-4.png|400](/img/user/6%20-%20Object/img/image-4.png)

> [!note]
> You can use line to connect (no need for ball and socket)

---

### 🎛️ Model–View–Controller (MVC)

> [!info]  
> Used in interactive applications that separate user interaction, data, and control logic.

**Components:**
- **Model:** Manages data & logic.
- **View:** Presents UI to user.
- **Controller:** Handles input & coordinates Model ↔ View.

![MVC-Architecture.webp|400](/img/user/6%20-%20Object/img/MVC-Architecture.webp)

![image-3.png|400](/img/user/6%20-%20Object/img/image-3.png)

**Flow:**  
1️⃣ User acts → Controller  
2️⃣ Controller updates Model  
3️⃣ Model notifies View  
4️⃣ View refreshes display

---

### Repository, Data-driven Systems

- Central **repository** acts as a shared data source.
- Multiple **components** (agents, services) access the repository to store, retrieve, and process data.

