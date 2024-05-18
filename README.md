### Self-Assessment: Onion Architecture, MVC, and Web API (.NET Core) with Bottlenecks

#### Conceptual Understanding:

**Onion Architecture:**
- **Have you heard of the Onion Architecture principle in software design?** 
  - Yes

**MVC Pattern:**
- **Are you familiar with the Model-View-Controller (MVC) pattern for building web applications?**
  - Yes

**Web API:**
- **Do you understand the concept of building RESTful APIs using ASP.NET Core Web API?**
  - Yes

#### Application & Bottlenecks:

**Onion Architecture:**

- **Benefits:**
  - Separation of concerns
  - Testability
  - Maintainability

- **Bottlenecks (Encountered):**
  - Yes
    - **Increased complexity for simple projects:** Implementing Onion Architecture can add unnecessary complexity to smaller projects where a simpler architecture would suffice.
    - **Difficulty finding developers familiar with the pattern:** Finding developers who are well-versed in Onion Architecture can be challenging, leading to potential onboarding and training hurdles.

**MVC:**

- **Components:**
  - **Model:** Represents the data and the business logic.
  - **View:** Handles the presentation layer, displaying the data to the user.
  - **Controller:** Manages user input and interacts with the model to update the view.

- **Bottlenecks (Encountered):**
  - Yes
    - **Tight coupling between Model and Controller:** This can make unit testing difficult as changes in the business logic (Model) often require corresponding changes in the Controller, leading to a ripple effect throughout the application.
    - **Logic changes rippling through the application:** Changes in one part of the application can necessitate changes in other parts, making maintenance and updates more challenging.

**Web API:**

- **Differences from MVC:**
  - Yes
    - **Traditional MVC applications** are typically used for creating web pages and include a full cycle of request and response with views and controllers. They handle both the user interface and the business logic.
    - **Web APIs** are designed for interaction with clients through RESTful endpoints, focusing on data exchange rather than rendering views. They provide a more lightweight approach for handling requests and responses, often used for mobile or SPA (Single Page Application) backends.

- **Bottlenecks (Encountered):**
  - Yes
    - **Frequent page refreshes causing performance overhead:** Traditional MVC applications can suffer from performance issues due to the need to refresh entire pages, which can be inefficient for dynamic data updates.
    - **Complex data exchange requiring a more lightweight approach:** Traditional MVC might not be the best fit for applications needing efficient, frequent, and complex data interactions. Web APIs provide a more streamlined and performant solution for these scenarios.
