# Alternative Way to Define and Create Routes.

1. Use the ```<Routes></Routes>``` component.
2. Inside the ```<Routes></Routes>``` component, create ```<Route></Route>``` components to define routes.
3. Declare the path and element as props to the ```<Route></Route>``` component.
4. element will have the value set to the component of that particular route to be visited.

```
<Routes>
    <Route path='/' element={<Users></Users>}></Route>
    <Route path='/users' element={<Users></Users>}></Route>
    <Route path='/about' element={<About></About>}></Route>
    <Route path='/contact' element={<Contact></Contact>}></Route>
</Routes>
```

5. Set BrowserRouter inside index.js file. 

```
<BrowserRouter>
      <App />
</BrowserRouter>
```

6. Now set the navlinks using the Link or NavLink tag on the header component and place the header component before the Routes component on App.js.

7. Routes component works as the outlet component here, representing all the children, whereas the header component remains to be the parent, which must be visible in every layout/screen/page.