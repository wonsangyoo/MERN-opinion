<h1>MERN Stack - Opinion Collector Backend API Specification</h1>

Created for backend with Node.js
Frontend will be created with React later.

<h2>Functionalities</h2>

<h3>Authentication</h3>
  <ul>
    <li>User Registration
      <ul>
        <li>Register as "admin" or general "user"</li>
        <li>Token should be sent once registration is successful</li>
        <li>2nd authentication via email*</li>
        <li>Password hashed</li>
      </ul>
    </li>
    <li>User login
      <ul>
        <li>Users log in with email and password</li>
        <li>Token should be sent once login is successful</li>
      </ul>
    </li>
    <li>User logout
      <ul>
        <li>Cookie sent - token=none</li>
      </ul>
    </li>    
    <li>Authentication
      <ul>
        <li>JWT/cookie</li> 
      </ul>
    </li>   
    <li>User info update
      <ul>
        <li>Authenticated user only</li>
        <li>Field validation via mongoose</li>
        <li>Separated route for password reset*</li>
      </ul>
    </li>    
    <li>User CRUD
      <ul>
        <li>Admin only, manually</li>
      </ul>
    </li>
    <li>Password lost
      <ul>
        <li>User can request to reset password</li>
        <li>User can request to reset password</li>
        <li>A put request can be made to the generated url to reset password</li>
        <li>The token will expire after 10 minutes</li>
      </ul>
    </li>
  </ul>

<h3>Surveys</h3>
<ul>
  <li>List all surveys
    <ul>
      <li>List surveys by category via navbar</li>
      <li>Pagination</li>
      <li>Limit number of results by page</li>
    </ul>
  </li>
  
  <li>Get single survey</li>
    
  <li>Create a new survey
    <ul>
      <li>Admin only</li>
    </ul>
  </li>
    
  <li>Update a survey
    <ul>
      <li>Admin only</li>
    </ul>
  </li>
  
  <li>Delete a survey
    <ul>
      <li>Admin only</li>
    </ul>
  </li>

</ul>

<h3>Opinions</h3>

<ul>
  <li>Submit opinion
    <ul>
      <li>Authenticated users and admin only</li>
      <li>Select rate(score) or y/n</li>
      <li>Optional opinion description</li>
      <li>Field validation via mongoose</li>
    </ul>
  </li>
  
  <li>List all opinion
    <ul>
      <li>Authenticated users and admin only</li>
      <li>Pagination</li>
    </ul>
  </li>
  
  <li>Update opinion
    <ul>
      <li>Authenticated users and admin only</li>
      <li>Select rate(score) or y/n</li>
      <li>Optional opinion description</li>
      <li>Field validation via mongoose</li>
    </ul>
  </li>
  
  <li>Delete opinion
    <ul>
      <li>Authenticated users and admin only</li>
    </ul>
  </li>
</ul>

<h3>Security</h3>
  <ul>
    <li>Encrypt passwords and reset tokens</li>
    <li>Prevent NoSQL injections</li>
    <li>Add headers for security (helmet)</li>
    <li>Prevent cross site scripting - XSS</li>
    <li>Add a rate limit for requests of 100 requests per 10 minutes</li>
    <li>Protect against http param polution</li>
  </ul>

<h3>Documentation</h3>
  <ul>
    <li>Use Postman to create documentation</li>
    <li>Use docgen to create HTML files from Postman</li>
    <li>Add html files as the / route for the api</li>
  </ul>

<h3>Deployment</h3>
