# dummy-ghapp-deployer
<h1>
Deployer of Probot app on AWS Lambda 
</h1>

<body>
  <main>
    <section>
      <h2> Create the AWS Function </h2>
        <p>
          The first step of our code is to create the function by using the "create.yml" action. In order to use this action you have to set some secrets :
        </p>
        <dl>
          <dt> Information for the authentication </dt>
          <dd> AWS_ACCESS_KEY_ID : you can find this information inside the IAM Configuration </dd>
          <dd> AWS_SECRET_ACCESS_KEY : you can find this information inside the IAM Configuration </dd>
          <dd> AWS_REGION : region for the auth </dd>
          <dt> Function settings </dt>
          <dd> AWS_FUNCTION_ROLE : the role for your function, you can create a role inside the IAM configuration. </dd>
          <dd> LAMBDA_FUNCTION : this will be the name of your future function </dd>
          <dt> Values for the environmental variables </dt>
          <dd> AWS_GHAPP_ID : the github app id </dd>
          <dd> AWS_GHAPP_WEBHOOK_SECRET : the webhook secret </dd>
          <dd> AWS_GHAPP_PRIVATE_KEY : the private key of your application </dd>
        </dl>
    </section>
  </main>
</body>
  <!-- 
the role <strong>MUST</strong> have this policy name : AWSLambdaBasicExecutionRole-ef626d56-30a2-426d-a215-50f10b8781e3
-->
