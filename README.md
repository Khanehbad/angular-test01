## hello engineer,

Angular User Management Project
Generated using Angular CLI version 19.2.8

Implementation Requirements (Following Clean Code Principles):

We want to display a list of users on a page

1. User Model
Path: `src/app/core/models/user/user.model.ts`
```
  id: number;
  name: string;
  email: string;
  website: string;
```
2. User Service Implementation
Path: `src/app/core/services/user/user.service.ts`
```
getAllUsers(): Observable<User[]> {
  // Should return an Observable of User array
  // Makes a GET request to the API endpoint
  // Include proper TypeScript typing
}
```
3. Component Structure
```
app/
    pages/
      user/
        user.component.html
        user.component.ts//UserComponent
        user.component.scss
```
Component Requirements:
Fetch user data from the service
Display data in a table format showing:
```
Name
Email
Website
```

4. Routing Configuration
Path: `src/app/app.routes.ts`
```
{
  path: 'users',
  component: UserComponent
},
{
  path: '',
  redirectTo: 'users',
  pathMatch: 'full'
}
```
5. CRUD Operations Implementation
Implement the following in `UserComponent`:
`
Create: Add new user/Update: Edit existing user/Delete: Remove user
`
6. Error Handling
Implement comprehensive error handling in `UserComponent` for all `CRUD` operations.

