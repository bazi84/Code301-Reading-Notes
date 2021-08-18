# Reading Notes 1
  **What is a Component?.**
  *A component architecture is a type of application architecture composed of independent, modular, and reusable building blocks called components.*

  ## - Object-oriented view
  ***A component is viewed as a set of one or more cooperating classes. Each problem domain class (analysis) and infrastructure class (design) are explained to identify all attributes and operations that apply to its implementation. It also involves defining the interfaces that enable classes to communicate and cooperate.***
  ## - Conventional view
  ***It is viewed as a functional element or a module of a program that integrates the processing logic, the internal data structures that are required to implement the processing logic and an interface that enables the component to be invoked and data to be passed to it.***


  ## - Process-related view
  ### n this view, instead of creating each component from scratch, the system is building from existing components maintained in a library. As the software architecture is formulated, components are selected from the library and used to populate the architecture.

  - A user interface (UI) component includes grids, buttons referred as controls, and utility components expose a specific subset of functions used in other components.

  - Other common types of components are those that are resource intensive, not frequently accessed, and must be activated using the just-in-time (JIT) approach.

  - Many components are invisible which are distributed in enterprise business applications and internet web applications such as Enterprise JavaBean (EJB), .NET components, and CORBA components.

  ## - Advantages
  - Ease of deployment − As new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole.

  - Reduced cost − The use of third-party components allows you to spread the cost of development and maintenance.

  - Ease of development − Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system.

  - Reusable − The use of reusable components means that they can be used to spread the development and maintenance cost across several applications or systems.

  - Modification of technical complexity − A component modifies the complexity through the use of a component container and its services.

  - Reliability − The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse.

  - System maintenance and evolution − Easy to change and update the implementation without affecting the rest of the system.

  - Independent − Independency and flexible connectivity of components. Independent development of components by different group in parallel. Productivity for the software development and future software development.

    ## What is Props?
  React is a component-based library which divides the UI into little reusable pieces. In some cases, those components need to communicate (send data to each other) and the way to pass data between components is by using props.
  “Props” is a special keyword in React, which stands for properties and is being used for passing data from one component to another.
  But the important part here is that data with props are being passed in a uni-directional flow. (one way from parent to child)

    ##  Using Props in React
    I will be explaining how to use Props step by step.
    Firstly, define an attribute and its value(data)
    Then pass it to child component(s) by using Props
    Finally, render the Props Data

    ### - Props stand for properties and is a special keyword in React
    ### - Props are being passed to components like function arguments
    ### - Props can only be passed to components in one-way (parent to child)
    ### - Props data is immutable (read-only)

  [My Readme file page](README.MD)

