```cs
[Test]
public void SignIn()
{
    Go.To<SignInPage>().
        Email.Set("admin@mail.com").
        Password.Set("abc123").
        SignIn.Click();
}

[SetUp]
public void SetUp()
{
    AtataContext.Configure().
        UseChrome().
        UseBaseUrl("https://demo.atata.io/").
        Build();
}
```