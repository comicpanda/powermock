### This version(1.6.4.RELEASE) can work with SpockFramework.

![PowerMock](powermock.png)

[![Build Status](https://travis-ci.org/jayway/powermock.svg)](https://travis-ci.org/jayway/powermock)

Writing unit tests can be hard and sometimes good design has to be sacrificed for the sole purpose of testability. Often testability corresponds to good design, but this is not always the case. For example final classes and methods cannot be used, private methods sometimes need to be protected or unnecessarily moved to a collaborator, static methods should be avoided completely and so on simply because of the limitations of existing frameworks.

PowerMock is a framework that extends other mock libraries such as EasyMock with more powerful capabilities. PowerMock uses a custom classloader and bytecode manipulation to enable mocking of static methods, constructors, final classes and methods, private methods, removal of static initializers and more. By using a custom classloader no changes need to be done to the IDE or continuous integration servers which simplifies adoption. Developers familiar with the supported mock frameworks will find PowerMock easy to use, since the entire expectation API is the same, both for static methods and constructors. PowerMock aims to extend the existing API's with a small number of methods and annotations to enable the extra features. Currently PowerMock supports EasyMock and Mockito.

When writing unit tests it is often useful to bypass encapsulation and therefore PowerMock includes several features that simplifies reflection specifically useful for testing. This allows easy access to internal state, but also simplifies partial and private mocking.

Please note that PowerMock is mainly intended for people with expert knowledge in unit testing. Putting it in the hands of junior developers may cause more harm than good.

## News
* 2015-10-02: PowerMock 1.6.3 has been released with support for EasyMock 3.2 as well as compatibility with ByteBuddy and various other fixes. See [change log](https://raw.githubusercontent.com/jayway/powermock/master/changelog.txt) for details.
* 2015-07-25: PowerMock has moved to GitHub. From now on the old <a href="https://code.google.com/p/powermock/">Google Code page</a> should not be used anymore. All issues are reported here on GitHub and the documentation is migrated.
* 2015-03-16: PowerMock 1.6.2 has been released. See [change log](https://raw.githubusercontent.com/jayway/powermock/master/changelog.txt) for details.

[Older News](https://github.com/jayway/powermock/wiki/OldNews)

## Documentation
* [Getting Started](https://github.com/jayway/powermock/wiki/GettingStarted)
* [Downloads](https://github.com/jayway/powermock/wiki/Downloads)
* [Motivation](https://github.com/jayway/powermock/wiki/Motivation)
* Javadoc
  * [EasyMock API extension](http://www.javadoc.io/doc/org.powermock/powermock-api-easymock/1.6.3) ([PowerMock class](http://static.javadoc.io/org.powermock/powermock-api-easymock/1.6.3/org/powermock/api/easymock/PowerMock.html))
  * [Mockito API extension](http://www.javadoc.io/doc/org.powermock/powermock-api-mockito/1.6.3) ([PowerMockito class](http://static.javadoc.io/org.powermock/powermock-api-mockito/1.6.3/org/powermock/api/mockito/PowerMockito.html))
  * [PowerMock Reflect](http://www.javadoc.io/doc/org.powermock/powermock-reflect/1.6.3) ([Whitebox class](http://static.javadoc.io/org.powermock/powermock-reflect/1.6.3/org/powermock/reflect/Whitebox.html))
* [EasyMock](https://github.com/jayway/powermock/wiki/EasyMock)
  * [Mock Static](https://github.com/jayway/powermock/wiki/MockStatic)
  * [Mock Final](https://github.com/jayway/powermock/wiki/MockFinal)
  * [Mock Private](https://github.com/jayway/powermock/wiki/MockPrivate)
  * [Mock New](https://github.com/jayway/powermock/wiki/MockConstructor)
  * [Mock Partial](https://github.com/jayway/powermock/wiki/MockPartial)
  * [Replay and verify all](https://github.com/jayway/powermock/wiki/ReplayAllAndVerifyAll)
* [Mockito](https://github.com/jayway/powermock/wiki/MockitoUsage) ([Legacy](https://github.com/jayway/powermock/wiki/MockitoUsage_Legacy))
* Common
  * [Bypass Encapsulation](https://github.com/jayway/powermock/wiki/BypassEncapsulation)
  * [Suppress Unwanted Behavior](https://github.com/jayway/powermock/wiki/SuppressUnwantedBehavior)
  * [Test Listeners](https://github.com/jayway/powermock/wiki/TestListeners)
  * [Mock Policies](https://github.com/jayway/powermock/wiki/MockPolicies)
  * [Mock system classes](https://github.com/jayway/powermock/wiki/MockSystem)
* [TestNG](https://github.com/jayway/powermock/wiki/TestNG_usage)
* [Delegate to another JUnit Runner](https://github.com/jayway/powermock/wiki/JUnit_Delegating_Runner)
* [Tutorial](https://github.com/jayway/powermock/wiki/PowerMock_tutorial)
* Experimental
  * [Bootstrap using a JUnit Rule](https://github.com/jayway/powermock/wiki/PowerMockRule)
  * [Bootstrap using a Java Agent](https://github.com/jayway/powermock/wiki/PowerMockAgent)
* [OSGi](https://github.com/jayway/powermock/wiki/osgi)
* [Release Notes](https://github.com/jayway/powermock/wiki/ReleaseNotes)
* [FAQ](https://github.com/jayway/powermock/wiki/FAQ) 

## Support and discussion
Join the mailing-list [here](http://groups.google.com/group/powermock) for questions, feedback and support.

## Links
* [Change log](https://raw.githubusercontent.com/jayway/powermock/master/changelog.txt)
* [PowerMock on Ohloh](http://www.ohloh.net/p/powermock/)
* [Mailing list for questions and support](http://groups.google.com/group/powermock)
 
## Sponsored by:
[![JAYWAY](http://www.arctiquator.com/oppenkallkod/assets/images/jayway_logo.png)](http://www.jayway.com/)

