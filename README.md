# spring-boot-complete-notes
## What is Spring Bean?
- Spring beans are regular **Java objects** that Spring takes care of. This means Spring handles their **creation**, **configuration**, and **lifecycle**.
- The IoC container is the heart of Spring bean management. It's responsible for creating beans, injecting dependencies into them, and ensuring they are available for use throughout your application.
  
**Benefits of Using Spring Beans:**
- **Reduce Boilerplate Code**: By letting Spring handle object creation and configuration, you write less code and focus more on the core functionality of your application's behavior.
- **Dependency Injection**: Spring beans can have their dependencies injected by the IoC container. This means you don't need to manually create and manages these dependencies, promoting loose coupling and testability in your code.

**How Spring Beans Work**
- **Bean Definition**: You provide Spring with instructions on how to create and configure beans. This can be done using XML configuration files (traditionally) or annotations in your java class.
- **Bean Creation**: The IoC container reads the bean definitions and uses them to instantiate the beans. It takes care of memory allocation and constructor calls.
- **Dependency Injection**: If a bean has dependencies, Spring injects them during bean creation. This removes the need of manual dependency management.
- **Bean Lifecycle Management**: Spring manages the lifecycle of beans, including initialization and destruction methods you might define in your bean classes.

## What is Spring Bean Definition?
- In spring, a bean definition acts as a **blueprint** for creating and managing a Spring bean. It provides the Spring IoC container with the information it needs to handle the bean's lifecycle.

A bean definition essentially stores configuration metadata about bean. This metadata dictates how the bean should be **created**, **configured** and **managed** by the IoC container.

**Details included.**
- Class
- Name
- Scope
- Constructor arguments
- Properties
- Autowiring mode
- Lazy initialization mode
- Initialization method
- Destruction method

| Resource | URL |
|----------|-----|
|Baeldung| https://www.baeldung.com/spring-bean |
|Spring.io| https://docs.spring.io/spring-framework/reference/core/beans/definition.html|
