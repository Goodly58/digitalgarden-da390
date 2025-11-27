---
{"dg-publish":true,"permalink":"/6-object/x-final-review/"}
---

# Midterm 1

#### Module 1

**Inheritance** 
New class (child) built on top of existing class (parent)

*Specialization: child class contains an attribute as an extra that does not exist in parent level.

![image-12.png|400x249](/img/user/6%20-%20Object/img/image-12.png)

**Abstraction**
Hiding complex logic from user.
![image-6.png|400x129](/img/user/6%20-%20Object/img/image-6.png)
Doesn't care about how calculateHealthIndex is calculated. Doctor just calls printDetails()

**Cohesion** (SERVE SINGLE PURPOSE?)
![image-7.png|400x230](/img/user/6%20-%20Object/img/image-7.png)
High cohesion: single responsibility delegating the math calculation to calculateHealthIndex(). and calculateHealthIndex() doesn't print only returns result of formula.

**Coupling** (HOW MANY CLASSES BREAK IF I CHANGE?)
![image-8.png|Here, you can see that Billing_tight will have an outdated formula if .calculateHealthIndex() formula changes.|400x250](/img/user/6%20-%20Object/img/image-8.png)


#### Module 2 UML

**Structural Diagrams**
![image-10.png|Class Diagram|400x268](/img/user/6%20-%20Object/img/image-10.png)

![image-11.png|Use Case Diagram|400x257](/img/user/6%20-%20Object/img/image-11.png)

> [!success]- Practice
> UML Use Case diagram • Draw a UML Use Case diagram for the details:
> 1. Customer browses catalog & selects items to buy
> 2. Customer goes to check out
> 3. Customer fills in shipping information
> 4. Customer fills in credit card information
> 5. The Credit card company authorizes purchase
> 
> > [!success]- Solution
> > ![image-15.png|400x191](/img/user/6%20-%20Object/img/image-15.png)
> 
> ![image-13.png|400x335](/img/user/6%20-%20Object/img/image-13.png)
> 
> > [!success]- Solution
> > ![image-14.png|400x420](/img/user/6%20-%20Object/img/image-14.png)
> 
> ![image-16.png|400x440](/img/user/6%20-%20Object/img/image-16.png)
> 
> > [!success]- Solution
> > ![image-17.png|400x328](/img/user/6%20-%20Object/img/image-17.png)
> > ![image-18.png|400x490](/img/user/6%20-%20Object/img/image-18.png)
> 
> ![image-19.png|400x376](/img/user/6%20-%20Object/img/image-19.png)
> 
> > [!success]- Solution
> > ![image-20.png|400x250](/img/user/6%20-%20Object/img/image-20.png)
> 
> ![image-21.png|400x216](/img/user/6%20-%20Object/img/image-21.png)
> 
> > [!success]- Solution
> > ![image-22.png|400x242](/img/user/6%20-%20Object/img/image-22.png)
> 

#### Module 4

| Type of Requirement | Meaning                                                                                               |
| ------------------- | ----------------------------------------------------------------------------------------------------- |
| Functional          | What system does (system must allow ...)                                                              |
| Non-functional      | Constraints/qualities:<br>- Performance (response time $<3$ s)<br>- Quality<br>- Safety<br>- Security |
| Domain              | Special constraints from the business world” (Business rules, laws, standards)                        |


# Midterm 2

⭐
![image-23.png|400x300](/img/user/6%20-%20Object/img/image-23.png)    
    1. **Architectural Design** (after doing requirements to create component model)
    2. **Interface Design** – how components talk to each other
    3. **Detailed Design**
	    - coding
	    - class diagram
		    - *Forward engineering*: diagram → code
		    - *Reverse engineering*: code → diagram

| Type                    | Simple idea                            | Example       |
| ----------------------- | -------------------------------------- | ------------- |
| **Interactive**         | User and system take turns             | ATM           |
| **Event-Driven**        | System acts when something happens     | Sensor system |
| **Transformational**    | Changes input into a new form          | Compiler      |
| **Database**            | Keeps and finds lots of data           | Oracle DB     |
| **Transaction based**   | Handles money/booking steps safely     | Banking app   |
| **Data driven systems** | Uses data to choose or suggest actions | Recommender   |


<span class="neon-highlight">UML Diagrams</span>
The SmartMed+ Remote Patient Monitoring System is a cloud-based healthcare solution developed to enable doctors to remotely monitor patients’ vital signs and respond quickly to emergencies. Each patient wears a SmartMed wearable device that continuously measures key health metrics such as heart rate, body temperature, and glucose levels. This device communicates via Bluetooth with a Mobile Gateway, typically the patient’s smartphone running the SmartMed Mobile App. The app encrypts and transmits the collected data through HTTPS to the Cloud Health Server, which hosts the SmartMed+ application and provides core functionalities such as health data storage, AI-driven anomaly detection, and alert notifications. The Cloud Server connects to a Database Server through a JDBC connection to store patient records, system logs, and doctor feedback. Doctors access the system through their Workstations or browser-based interfaces linked to the Cloud Server, while a System Administrator operates through an Admin Console Node to configure accounts, maintain data security, and monitor network operations.

*Tasks*
**Deployment Diagram** (architectural diagram)
Construct a Deployment Diagram illustrating all physical nodes and software artifacts in the SmartMed+ system. Include the SmartMed Device, Mobile Gateway, Cloud Health Server, Database Server, Doctor Workstation, and Admin Console Node. Clearly indicate the communication protocols (e.g., Bluetooth, HTTPS, JDBC) and deployment of artifacts such as SmartMed.apk, HealthAnalytics.jar, and PatientDB. Represent the logical relationships and communication links between all nodes.

**Communication Diagram**
Using the same scenario, model the message interactions among system components during the “Monitor Patient Health and Send Alert” process. Represent the participating objects—SmartMed Device, Mobile App, Cloud Server, Database, and Doctor Portal—and number the messages in logical order. Show data transmission from the device to the mobile app, data upload to the cloud, storage in the database, invocation of the AI analysis module, detection of abnormal readings, alert notification to the doctor, doctor feedback submission, and confirmation message to the patient’s app.

**Sequence Diagram**
Develop a Sequence Diagram for the same use case, showing the chronological flow of control and data. Begin with the device measuring and sending vital data to the Mobile App, followed by the app’s synchronous request to the Cloud Server. Include the server’s interaction with the Database and AI Analytics module, the asynchronous alert sent to the Doctor Portal, and the doctor’s response message with feedback or prescriptions. End the sequence with the Cloud Server storing the doctor’s feedback and sending a confirmation response to the Mobile App. Ensure that all lifelines, activation bars, synchronous and asynchronous messages, and return flows are semantically and syntactically correct.

> [!success]- Solution
> ![image-24.png|400x381](/img/user/6%20-%20Object/img/image-24.png)
> ![image-25.png|400x207](/img/user/6%20-%20Object/img/image-25.png)
> ![image-26.png|400x192](/img/user/6%20-%20Object/img/image-26.png)

<span class="neon-highlight">Architectural Diagram</span>
**Deployment Diagram**

**Component Diagram**
![image-43.png|300](/img/user/6%20-%20Object/img/image-43.png)

<span class="neon-highlight">Architectural Patterns</span> ⭐

Draw all the Architectural Patterns
> [!success]- Solution
> ![image-41.png|400x322](/img/user/6%20-%20Object/img/image-41.png)
> 
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/6-object/architectural-patterns/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">





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



</div></div>


# Post-M2

<span class="neon-highlight">DESIGN PATTERNS</span> ⭐

Link: [[6 - Object/Design Patterns\|Design Patterns]]

Draw all the design patterns
> [!success]- Solution
> TO DRAW: 
> **STRUCTURAL**: Composite, Decorator, Adapter, Facade, Proxy
> **BEHAVIORAL**: Observer, Iterator
> 

<span class="neon-highlight">TESTING</span> ⭐
Mapping input → output

![unnamed-1.jpg|3 types of testing|400x218](/img/user/6%20-%20Object/img/unnamed-1.jpg)

![unnamed-4.jpg|400x370](/img/user/6%20-%20Object/img/unnamed-4.jpg)
- If you change: value, order, ASCII, data type — ANYTHING AT ALL → new test case. 
> [!info]- original image
> ![Untitled-4.jpg|400x372](/img/user/6%20-%20Object/img/Untitled-4.jpg)



![unnamed.jpg|400x370](/img/user/6%20-%20Object/img/unnamed.jpg)

> [!example]- Code
> ```cpp
> public class AverageTest {
>     // Function to compute average
>     public static double average(int a, int b, int c) {
>         long sum = (long) a + b + c;  // avoid overflow
>         return sum / 3.0;
>     }
> 
>     // Modified assertEquals: prints result instead of throwing exception
>     private static void assertEquals(double expected, double actual, String testName) {
>         if (expected == actual) {
>             System.out.println(testName + " passed.");
>         } else {
>             System.out.println(testName + " failed: expected " + expected + " but got " + actual);
>         }
>     }
> 
>     public static void main(String[] args) {
> 
>         // Test cases
>         assertEquals(3.0, average(1, 2, 3), "Test 1: all positive");
>         assertEquals(0.0, average(0, 0, 0), "Test 2: all zeros");
>         assertEquals(-5.0, average(-4, -5, -6), "Test 3: all negative");
>         assertEquals(200000.0, average(100000, 200000, 300000), "Test 4: large integer values");
> 
>         System.out.println("All tests executed.");
>     }
> }
> ```

![unnamed-3.jpg|400x218](/img/user/6%20-%20Object/img/unnamed-3.jpg)

> [!example]- Code
> ```cpp
> public class ReverseStringSimple {
>     public static String reverse(String s) {
>         if (s == null) return null;
>         return new StringBuilder(s).reverse().toString();
>     }
> 
>     // Modified assertions: print result instead of throwing
>     private static void assertEquals(String testName, String expected, String actual) {
>         if (expected.equals(actual)) {
>             System.out.println(testName + " passed.");
>         } else {
>             System.out.println(testName + " failed: expected \"" + expected + "\", got \"" + actual + "\"");
>         }
>     }
> 
>     private static void assertTrue(String testName, boolean condition) {
>         if (condition) {
>             System.out.println(testName + " passed.");
>         } else {
>             System.out.println(testName + " failed: condition is false");
>         }
>     }
> 
>     private static void assertNotNull(String testName, Object obj) {
>         if (obj != null) {
>             System.out.println(testName + " passed.");
>         } else {
>             System.out.println(testName + " failed: object is null");
>         }
>     }
> 
>     private static void assertNull(String testName, Object obj) {
>         if (obj == null) {
>             System.out.println(testName + " passed.");
>         } else {
>             System.out.println(testName + " failed: object is not null");
>         }
>     }
> 
>     public static void main(String[] args) {
>         String str = "abcdefg";
> 
>         // All tests will run regardless of pass/fail
>         assertEquals("Test 1: reverse content", "gf", reverse(str)); // this will fail
>         assertTrue("Test 2: first character check", reverse(str).charAt(0) == 'g');
>         assertNotNull("Test 3: not null check", reverse(str));
>         assertNull("Test 4: null input check", reverse(null));
>         assertTrue("Test 5: length check", reverse(str).length() == 7);
> 
>         System.out.println("All tests executed.");
>     }
> }
> ```



<span class="neon-highlight">RDCT</span> ⭐
![unnamed-1-1.jpg|400x218](/img/user/6%20-%20Object/img/unnamed-1-1.jpg)

<span class="neon-highlight">Software development process model </span> ⭐
1. plan-driven (waterfall)
2. incremental (agile)
	1. XP (Extreme Programming) → finish software as fast as possible ![image-39.png|highest priority task should be implemented first|400x196](/img/user/6%20-%20Object/img/image-39.png)	practices:
			- Code **refactoring**: cleaning code.
			- Small frequent releases
			- test-first development
	
3. Rational Unified Processing model
	![image-44.png|i.e. steps of software engineering (midterm 1) |400x148](/img/user/6%20-%20Object/img/image-44.png)
	
![Untitled-5.jpg|400x533](/img/user/6%20-%20Object/img/Untitled-5.jpg)
**Agile**: rapid development, rapid collection of feedback. Phases can overlap *(Sprint 1 could have 20% R andHow scaling is used in k means.

Final is compreehnsive (but she wont ask things like build decision tree). Scaling si important, but u wont need to scale dataset. She will send a post about it. Focus is material not covered in the midterm.




 20% D)*
**Plan-driven**: slower development, slower collection of feedback

NASA, medical, or other critical time software (large size software) are water-fall or agile?
> [!success]- Solution
> It is very risky to move to design. You need to understand requirements fully.

SDLC: Which one is most costly phase? Least?
> [!success]- Solution
> Maintenance (last phase of SDLC → software development life cycle) is most expensive because it's too late.
> Requirement (first phase of SDLC) is least. 

SDLC: What is the most critical phase?
> [!success]- Solution
> The most critical phase is requirement. It is written in natural language and thus there can be confusion between the requirement team and the design team. 


<span class="neon-highlight">Test-driven development</span>
Number of test cases:$2^{number of input}$


---

# Final Hints
In final exam (comprehensive):
1. conceptual scenario. 1-2paragraphs. based on analyzing scenario, sketch closest design pattern (composite, facade), sketch class diagram, might ask to generate code.
2. Give you source code, based on that what is the closest design pattern.
3. (Code is for design patterns and code for abstraction, encapsulation, etc.)

1 theoretical question (likely post-m2)