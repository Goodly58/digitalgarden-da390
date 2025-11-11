---
{"dg-publish":true,"permalink":"/4-web-app/java-quiz-2-prep/"}
---


![image-7.png|400](/img/user/4%20-%20Web%20app/img/image-7.png)

> [!success]- Solution
> Child show()

### **Question 2**

What is the output?

```java
class Base {
    Base() {
        System.out.println("Base Constructor");
    }
}

class Derived extends Base {
    Derived() {
        System.out.println("Derived Constructor");
    }
}

public class Test {
    public static void main(String[] args) {
        Derived d = new Derived();
    }
}
```

> [!success]- Solution  
> ✅ **Output:**
> 
> ```
> Base Constructor
> Derived Constructor
> ```
> 
> Java automatically adds `super()` as the first line of every subclass constructor.

---

### **Question 3**

What is the output?

```java
abstract class Shape {
    abstract void draw();
}

class Square extends Shape {
    void draw() {
        System.out.println("Drawing Square");
    }
}

public class Demo {
    public static void main(String[] args) {
        Shape s = new Shape();
        s.draw();
    }
}
```

> [!success]- Solution  
> ❌ **Compilation error**  
> You **cannot instantiate** an abstract class directly.  
> Only subclasses that implement `draw()` can be instantiated.

---

### **Question 4**

What will be printed?

```java
class Parent {
    void greet() {
        System.out.println("Hello from Parent");
    }
}

class Child extends Parent {
    void greet(String msg) {
        System.out.println(msg);
    }
}

public class Demo {
    public static void main(String[] args) {
        Parent p = new Child();
        p.greet();
    }
}
```

> [!success]- Solution  
> ✅ **Output:** `Hello from Parent`  
> The `Child` class **overloads** `greet()` (different parameters) — not **overrides** it.  
> Hence, `Parent` version is called.

---

### **Question 5**

What will be the output?

```java
public class Test {
    public static void main(String[] args) {
        try {
            int x = 5 / 0;
            System.out.println("Result: " + x);
        } catch (ArithmeticException e) {
            System.out.println("Division by zero!");
        } finally {
            System.out.println("Finally block executed.");
        }
    }
}
```

> [!success]- Solution  
> ✅ **Output:**
> 
> ```
> Division by zero!
> Finally block executed.
> ```
> 
> The `catch` block handles the error, and the `finally` block **always executes**.
> <span class="neon-highlight">This is a compile time error</span>

> [!success]- What if we changed 5 / 0 → a / b (where a=5,b=0)
> “It still throws an `ArithmeticException` at **runtime**, but the `catch` handles it. Without the try–catch, it would be a runtime error that crashes the program.”

---

### **Question 6**

Explain constructor calling order when multiple classes are inherited.

```java
class Parent {
    Parent() { System.out.println("Parent"); }
}
class Child1 extends Parent {
    Child1() { System.out.println("Child1"); }
}
class Child2 extends Child1 {
    Child2() { System.out.println("Child2"); }
}
class Child3 extends Child2 {
    Child3() { System.out.println("Child3"); }
}
public class Demo {
    public static void main(String[] args) {
        new Child3();
    }
}
```

> [!success]- Solution  
> ✅ **Output:**
> 
> ```
> Parent
> Child1
> Child2
> Child3
> ```
> 
> - Each child constructor calls its parent’s constructor first (`super()` is implicit).
>     
> - The order of execution goes **top-down**, but the **calls** happen **bottom-up**:  
>     `Child3 → Child2 → Child1 → Parent` (calls)  
>     → prints **Parent → Child1 → Child2 → Child3**.
>     



---

## 🧠 Java Exam Practice (Q7–Q20)


### **Q8**

> [!question]
> What’s the output?

```java
class A {}

class B {
    B(int x) { System.out.println("B: " + x); }
}

public class Main {
    public static void main(String[] args) {
        A a = new A();
        B b = new B();
        System.out.println("Done");
    }
}
```

> [!success]- Solution
> Compilation error
> ![image-3.png](/img/user/4%20-%20Web%20app/img/image-3.png)

---

### **Q9**

> [!question]
> What’s the output?

```java
class Parent {
    Parent(int n) { System.out.println("Parent: " + n); }
}

class Child extends Parent {
    Child() { System.out.println("Child"); }
}

public class Main {
    public static void main(String[] args) {
        new Child();
    }
}
```

> [!success]- Solution
> Compilation error
> > [!success]- How do you fix it?
> > 1. Call existing constructor explicitly (e.g. super(5))
> > 2. Make a default constructor in Parent
> > 3. Remove parametized constructor in Parent

---

### **Q10**

> [!question]
> What’s the output if you create a dog object?

```java
class Pet {
    Pet() { System.out.println("Pet ctor"); }
}

class Dog extends Pet {
    Dog() {
        System.out.println("Hello");
        super();
    }
}
```

> [!success]- Solution
> Compilation error. <span class="neon-highlight">super() must be first line of constructor</span>.

---

### **Q11**

> [!question]
> What’s the output?

```java
class Pet { void speak() { System.out.println("Pet speaking"); } }
class Dog extends Pet { void speak() { System.out.println("Dog speaking"); } }

public class Main {
    public static void main(String[] args) {
        Pet p = new Dog();
        p.speak();
    }
}
```

> [!success]- Solution
> Dog speaking

---

### **Q12**

> [!question]
> What’s the output?

```java
class Pet {}
class Dog extends Pet { void bark() { System.out.println("Woof"); } }
class Cat extends Pet {}

public class Main {
    public static void main(String[] args) {
        Pet[] pets = { new Dog(), new Cat() };
        for (Pet p : pets) {
            if (p instanceof Dog)
                p.bark();
        }
        System.out.println("Done");
    }
}
```

> [!success]- Solution
> Compilation error

> [!question]
> What’s the output?

```java
class Pet {}
class Dog extends Pet { void bark() { System.out.println("Woof"); } }
class Cat extends Pet {}

public class Main {
    public static void main(String[] args) {
        Pet[] pets = { new Dog(), new Cat() };
        for (Pet p : pets) {
	        ((Dog)p).bark();
        }
        System.out.println("Done");
    }
}
```

> [!success]- Solution
> Runtime error

---

### **Q13**

> [!question]
> What’s the output?

```java
class Pet {
    static void info() { System.out.println("Pet info"); }
    void speak() { System.out.println("Pet speaking"); }
}
class Dog extends Pet {
    static void info() { System.out.println("Dog info"); }
    void speak() { System.out.println("Dog speaking"); }
}
public class Main {
    public static void main(String[] args) {
        Pet p = new Dog();
        p.info();
        p.speak();
    }
}
```

> [!success]- Solution
> Pet info
> Dog speaking
> >[!note]
> >Static methods are not polymorphic in Java. Static methods do static binding (compile-time binding. So use type on the left). Non-static or dynamic methods do dynamic binding (run-time binding. So use type on the right).
> > `<Static> p = new <Dynamic>();`
> > `Parent p = new Child();`
>
> > [!question]- Why didn't we downcast here?
>  Because both speak() and info() exist in Pet class

> [!success]- Why do we do static in general?
> ![image-4.png](/img/user/4%20-%20Web%20app/img/image-4.png)

---

### **Q14**

> [!question]
> What’s the output?

```java
class Secret {
    private Secret() { System.out.println("Secret made"); }
}
public class Main {
    public static void main(String[] args) {
        new Secret();
    }
}
```

> [!success]- Solution
> Compilation error

---

### **Q15**

> [!question]
> What’s the output if you create an object of child class?

```java
class Grand { Grand() { System.out.println("Grand"); } }
class Parent extends Grand { Parent() { System.out.println("Parent"); } }

class Child extends Parent {
    Child() {
        super.super();
        System.out.println("Child");
    }
}
```

> [!success]- Solution
> Compilation error. You can only use super() or super.someMethod().
> > [!success]- Output if we call super()?
> > Grand → Parent → Child

---

### **Q16**

> [!question]
> What’s the output?

```java
class Base {
	static int x=5;
}
public class Main {
    public static void main(String[] args) {
	    System.out.println(Base.x);
    }
}
```

> [!success]- Solution
> 5.
> If it was non-static, it wouldn't run.

> [!question]
> What’s the output?

```java
class Base {
    abstract void go();
}

class Child extends Base {
    void go() {
        System.out.println("Child go");
    }
}

public class Main {
    public static void main(String[] args) {
        Child c = new Child();
        c.go();
    }
}
```


> [!success]- Solution  
> Compilation error
> 
> Even though:
> 
> - `Child` correctly implements `go()`
>     
> - `main` only uses `Child` and `Base.x` (both fine)
>     
> 
> This line is still illegal:
> 
> ```java
> class Base {
>     abstract void go();
> }
> ```
> 
> A class with an abstract method **must** be declared `abstract`, so it should be:
> 
> ```java
> abstract class Base { ... }
> ```

---

### **Q17**

> [!question]
> What’s the output?

```java
interface Pet {
    int I = 6;
    void play();
}
public class Main {
    public static void main(String[] args) {
        Pet p = new Pet();
        System.out.println(Pet.I);
    }
}
```

> [!success]- Solution
> Compilation error
> Pet p = new Pet();          // ❌
> System.out.println(Pet.I);  // ✅
> You can't create an object for interfaces.


---

### **Q18**

> [!question]
> What’s the output?

```java
interface Consts {
    int MIN_VOTING_AGE = 18;
}
public class Main {
    public static void main(String[] args) {
        System.out.println(Consts.MIN_VOTING_AGE);
    }
}
```

> [!success]- Solution
> 18
>
> > [!success]- What is the keywords Java assigns to the attribute of Consts?
> > `Public` → accessible from anywhere
> > `Static` → belong to interface itself, not object
> > `Final` → constant, cannot be changed

---

### **Q19**

> [!question]
> What’s the output?

```java
class Parent {}
class Child extends Parent {}

public class Main {
    public static void main(String[] args) {
        Child c = new Parent();
        Parent p = new Child();
        System.out.println("OK");
    }
}
```

> [!success]- Solution
> Compilation error
> `Child c = new Parent();` doesn't work

---

### **Q20**

> [!question]
> What’s the output?

```java
class Parent {
    Parent() { System.out.println("Parent"); }
}
class Child extends Parent {
    Child() { System.out.println("Child"); }
}
public class Main {
    public static void main(String[] args) {
        new Child();
    }
}
```

> [!success]- Solution
> Parent
> Child


---
## File stream: What's missing?

---

### **Q1**

```java
public class WriteFile {
    public static void main(String[] args) {
        FileOutputStream out = new FileOutputStream("notes.txt");
        out.write(65);
    }
}
```

> [!question]  
> The code intends to write a single character into a file. What’s missing?

> [!success]- Solution
> - Must **handle exception** using `try-catch` or `throws IOException`.
>     
> - Must **close the stream** after writing: `out.close();`
>     

---

### **Q2**

```java
public class WriteData {
    public static void main(String[] args) throws IOException {
        File file = new File("data.txt");
        FileOutputStream out = new FileOutputStream(file);
        String text = "Hello File!";
        byte[] b = text.getBytes();
        out.write(b);
    }
}
```

> [!question]  
> The program runs but the file stays locked after execution. What’s missing?

> [!success]- Solution  
> You must **close the output stream**:
> 
> ```java
> out.close();
> ```
> We didn't need to do try catch cause we used "throws IOException"

---

### **Q3**

```java
File file = new File("log.txt");
FileOutputStream fout = new FileOutputStream(file, true);
String text = "New line";
fout.write(text.getBytes());
System.out.println("Written successfully");
```

> [!question]  
> The code throws “unreported exception IOException.” What’s missing?

> [!success]- Solution
> 
> - Must handle or declare the **checked exception** (`IOException`).  
>     Either wrap in `try-catch(IOException e)` or add `throws IOException` to the method.
> - `fout.close()`
>     

---

### **Q4**

```java
public class ReadFile {
    public static void main(String[] args) throws IOException {
        FileInputStream in = new FileInputStream("notes.txt");
        int i;
        while (i != -1) {
            i = in.read();
            System.out.print((char) i);
        }
        in.close();
    }
}
```

> [!question]  
> The code doesn’t compile because of the variable _i_. What’s missing?

> [!success]- Solution  
> The variable `i` must be **initialized before use**.  
> Correct:
> 
> ```java
> int i = in.read();
> while (i != -1) {
>     System.out.print((char)i);
>     i = in.read();
> }
> ```
> FIX using either:
> 1. do while loop
> 2. initialize i before the loop (because you cant do if condition when i doesn't have a value set). If you do this, you have to move i=in.read() too.

---

### **Q5**

```java
File f = new File("report.txt");
if (!f.exists())
    System.out.println("File created!");
```

> [!question]  
> What’s missing?

> [!success]- Solution  
> The `File` object only represents the file — it doesn’t create it.  
> Must call:
> 
> ```java
> f.createNewFile();
> ```

---

### **Q6**

```java
try {
    FileOutputStream out = new FileOutputStream("output.txt");
    out.write(65);
    System.out.println("Done");
} finally {
    System.out.println("Closing...");
    out.close();
}
```

> [!question]  
> Compilation error: “out cannot be resolved.” What’s missing?

> [!success]- Solution  
> Declare the stream **outside the try block** so it’s visible in `finally`:
> 
> ```java
> FileOutputStream out = null;
> try {
>     out = new FileOutputStream("output.txt");
>     out.write(65);
> } finally {
>     if (out != null) out.close();
> }
> ```


> [!success]- In fileIO, what are the functions that need try-catch blocks?
> 
> 1. **Creating byte/char streams**
>     
>     ```java
>     new FileInputStream("x.txt");
>     new FileOutputStream("x.txt");
>     new FileReader("x.txt");
>     new FileWriter("x.txt");
>     ```
>     
> 2. **Reading**
>     
>     ```java
>     in.read();        // from InputStream / Reader
>     in.available();   // from InputStream
>     ```
>     
> 3. **Writing**
>     
>     ```java
>     out.write(65);
>     out.write(bytes);
>     out.flush();
>     ```
>     
> 4. **Closing streams**
>     
>     ```java
>     in.close();
>     out.close();
>     reader.close();
>     writer.close();
>     ```
>     
> 5. **Creating a file with `File`**
>     
>     ```java
>     f.createNewFile();
>     ```
>     

> [!success]- What doesn't need?
> File and file methods, with the exception of File.createNewFile()
> (as compared to those that need which are FileInputStream, FileOutputStream, FileReader, FileWriter)
> ![image-6.png](/img/user/4%20-%20Web%20app/img/image-6.png)

---

### **Q7**

```java
FileInputStream in = new FileInputStream("data.txt");
int i;
while ((i = in.read()) != -1)
    System.out.print((char)i);
in.close();
```

> [!question]  
> What import or handling is missing here?

> [!success]- Solution
> 
> - Must **import java.io.***
>     
> - Must **handle or declare IOException** since `FileInputStream` and `read()` throw checked exceptions.
>     

---

### **Q8**

```java
try {
    FileInputStream fin = new FileInputStream("data.txt");
    int i;
    while((i = fin.read()) != -1)
        System.out.print((char)i);
}
catch(Exception e) {
    System.out.println("Error reading file");
}
```

> [!question]  
> The file stays open even after finishing the loop. What’s missing?

> [!success]- Solution  
> Must **close the stream** after reading:
> 
> ```java
> finally {
>     fin.close();
> }
> ```
> 

> [!success]- What counts as opening the file?
> ![image-5.png](/img/user/4%20-%20Web%20app/img/image-5.png)

---

### **Q9**

```java
File f = new File("text.txt");
FileOutputStream out = new FileOutputStream(f);
out.write("Hi".getBytes());
```

> [!question]  
> Program compiles but terminates abruptly with an exception. What’s missing?

> [!success]- Solution  
> The **file path or permission** might not exist.  
> Must handle **FileNotFoundException** using:
> 
> ```java
> try { ... } catch (FileNotFoundException e) { ... }
> ```
>
> also .close() is missing 

---


### **Q10**

```java
try {
    FileReader fr = new FileReader("data.txt");
    int c;
    while ((c = fr.read()) != -1)
        System.out.print((char)c);
}
catch (IOException e) {
    System.out.println("Error reading file");
}
```

> [!question]  
> What’s missing if this should use _character-based streams correctly_?

> [!success]- Solution  
> Must **close the reader**

---

### **Q12**

```java
FileOutputStream fout = new FileOutputStream("output.txt");
String data = "Welcome";
fout.write(data);
fout.close();
```

> [!question]  
> The code doesn’t compile. What’s missing?

> [!success]- Solution  
> `write()` expects a **byte array**, not a string.  
> Must convert using `getBytes()`:
> 
> ```java
> fout.write(data.getBytes());
> ```

---


> [!note]

<table>
  <thead>
    <tr>
      <th>Topic</th>
      <th>Summary</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><b>File vs Streams</b></td>
      <td>
        <ul>
          <li><code>File</code> = path info only, does <b>not</b> open the file.</li>
          <li><code>FileInputStream / FileOutputStream / FileReader / FileWriter</code> = real I/O (open the file).</li>
        </ul>
      </td>
    </tr>

    <tr>
      <td><b>Needs try/catch</b></td>
      <td>
        <ul>
          <li>Creating streams: <code>new FileInputStream(...)</code>, <code>new FileOutputStream(...)</code>, <code>new FileReader(...)</code>, <code>new FileWriter(...)</code></li>
          <li>I/O ops: <code>read()</code>, <code>write()</code>, <code>flush()</code>, <code>close()</code></li>
          <li><code>File.createNewFile()</code></li>
        </ul>
      </td>
    </tr>

    <tr>
      <td><b>Does NOT need try/catch</b></td>
      <td>
        <ul>
          <li><code>new File("x.txt")</code></li>
          <li>Common <code>File</code> methods: <code>exists()</code>, <code>isFile()</code>, <code>isDirectory()</code>, <code>canRead()</code>, <code>canWrite()</code>, <code>length()</code>, <code>getName()</code>, <code>getPath()</code>, <code>delete()</code>, <code>renameTo(...)</code></li>
        </ul>
      </td>
    </tr>

    <tr>
      <td><b>Open & Close</b></td>
      <td>
        <ul>
          <li>Open = creating stream: <code>new FileInputStream(...)</code>, <code>new FileOutputStream(...)</code>, etc.</li>
          <li>Always <code>close()</code> streams when done.</li>
          <li>Put <code>close()</code> in <code>finally</code> so it runs even if an exception happens.</li>
        </ul>
      </td>
    </tr>

    <tr>
      <td><b>Reading pattern</b></td>
      <td>
        <pre><code>int i = in.read();
while (i != -1) {
    System.out.print((char)i);
    i = in.read();
}</code></pre>
        <ul>
          <li>Local <code>int i</code> must be initialized before first use.</li>
        </ul>
      </td>
    </tr>

    <tr>
      <td><b><code>flush()</code></b></td>
      <td>
        <ul>
          <li>Forces buffered data to be written <b>now</b>, stream stays open.</li>
          <li><code>close()</code> flushes automatically; use <code>flush()</code> when you want data written but are not closing yet.</li>
        </ul>
      </td>
    </tr>

    <tr>
      <td><b>Cheat line</b></td>
      <td>
        <ul>
          <li><b>File</b> = path, no try/catch (except <code>createNewFile()</code>).</li>
          <li><b>Streams</b> = real I/O → need try/catch / <code>throws</code> and must be <code>close()</code>d.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
