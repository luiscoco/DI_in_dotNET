# DI_in_dotNET

https://learn.microsoft.com/en-us/dotnet/core/extensions/dependency-injection-usage?source=recommendations

This tutorial shows how to use dependency injection (DI) in .NET. With Microsoft Extensions, DI is managed by adding services and configuring them
in an IServiceCollection. The IHost interface exposes the IServiceProvider instance, which acts as a container of all the registered services.

In this tutorial, you learn how to:

Create a .NET console app that uses dependency injection
Build and configure a Generic Host
Write several interfaces and corresponding implementations
Use service lifetime and scoping for DI

In this sample app, you created several interfaces and corresponding implementations. Each of these services is uniquely identified and paired with a ServiceLifetime. The sample app demonstrates registering service implementations against an interface, and how to register pure classes without backing interfaces. The sample app then demonstrates how dependencies defined as constructor parameters are resolved at run time.

From the app output, you can see that:

- Transient services: are always different, a new instance is created with every retrieval of the service.
- Scoped services: change only with a new scope, but are the same instance within a scope.
- Singleton services: are always the same, a new instance is only created once.
