# Requirements

### What is the vision of this product?

> Uncle Jimmy’s Life Coaching. Get life advice from your AI-powered Uncle Jimmy. Advice/tasks given can be saved to your “Life Improvement List”. Snark and sarcasm included at no additional charge.

### What pain point does this project solve?

1. Provides free life advice
2. Allows tracking of life improvement task list
3. Provides entertainment through light-hearted humor

### Why should we care about your product?

It is entertaining and educational to make your life more productive and satisfying

## Scope (In/Out)

### IN - What will your product do

1. Users can get an AI-generated recommendation based on prompt input
2. Users can add a generated recommendation to their own private task list
3. Users can view and delete items from their list
4. Users can add and edit notes under each item
5. Users can mark an item as complete

### OUT - What will your product not do.

1. The application will not function as a native application on any platform

### MVP functionality

1. Get an AI-generated recommendation based on user prompt
2. Add recommendation to task list (create)
3. Ability to view, edit (complete or notate) and delete items from the list

### What are your stretch goals?

1. Lifecoach will make additional recommendations based off of users task lists
2. User can input their own custom tasks
3. User profile
4. Search/filter task list

### Functional Requirements

1. Users can get an AI-generated recommendation based on prompt input
2. Users can add a generated recommendation to their own private task list
3. Users can view and delete items from their list
4. Users can add and edit notes under each item
5. Users can mark an item as complete

#### Data Flow

User logs in to their profile using a social login. If new user, an empty profile will be created. If existing, previous tasks will load in to their personal list.

User will be greeted by a minimalist page with an input to ask for advice from the lifecoach. Once user submits their request, a task will be generated and added to their list.

User can then view their list of tasks and select one to view or mark as completed. If they open it to view, they can see their notes to add or update, as well as the option to delete or complete the task.

User has the option to sign out when finished with the expectation that thier data will persisit when they return again.

#### Non-Functional Requirements

* Security
  * We will ensure that proper authentication is implemented to varify the user is who they say they are
  * We will ensure that the user can only access their own data for privacy
  * APIs will only work with authenticated users
* Testability
  * We will create a live development deployment where we can test all features as they are implemented prior to deployment to production
  * We will verify:
    * Users can sign in/out
    * Users can only see their own data
    * Users can only modify data that pertains to their account
    * Users can always get a response from the life coach to create a new task
