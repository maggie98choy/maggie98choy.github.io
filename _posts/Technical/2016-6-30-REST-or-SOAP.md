---
layout: post
title: REST vs SOAP
tags: 
- Web Services
- REST
- SOAP
published: true
categories:
- Technical
---

I've been developed several SOAP and REST web services applications in the past. I know pretty well of how to develop a 
web services application using both SOAP or REST approach. Recently, someone asked me why I choose this approach over 
another. I told them if you have specific requirement and reason use SOAP otherwise use REST. The person didn't seem satisfied. So I did some homework and here is the summary of SOAP aand REST.

Let's tell a little background of both technologies before going into the reasons of choosing which approach for application.

### SOAP
SOAP(Simple Object Access Protocol) was developed by Microsoft for the purpose of replacing older web technologies DCOM 
(Distributed Component Object Model) and COBRA (Common Object Request Broker Architecture) that didn't work well on Internet.
SOAP is a mature web technology protocol that exposes individual operation as web services. It's rely exlusively on XML to define content of message. SOAP focuses on accessing name operation while each implement business logic through interfaces.

### REST
Many developers found tiresome to develop code for SOAP. For example, develop SOAP web service using Javascript require to write ton of code just to achieve simple task because we must create XML structure every time. REST is a light weight alternative to SOAP. Instead of relying on XML for exchanging message it uses URL approach. REST focuses on resource-based operation. It inherits CRUD (POST, GET, PUSH, DELETE) from HTTP operations. This make it easy for both developer and browser to consume public APIs as you have no control over on what's going on the consumer side. This is one of the main reason REST dominant nearly 70% of the market.

## Advantages of SOAP over REST
1. SOAP supports SSL (REST also provides this feature) and WS-Security which offers enterprise security features to system. This feature provides add on data privacy and data security.
2. SOAP provide realiable end-to-end built-in error handling feature. This feature is useful for enterprise application that require high level of transaction reliability. REST does not have built-in error handling feature so client side has to deal with failure operation.

## Advantages of REST over SOAP
1. Simplicity. REST is rather easy to learn and develop. Creating clients, developing APIs and understanding of documentation of REST are much easier than SOAP. REST uses HTTP protocol and inherits CRUD operation from it so it is much simpler.
2. REST supports not only XML messaging format but also JSON and CSV output format. This give developer flexibility of choosing which output format to use depending on the language of application. JSON is usually the better fit for data structure as it is much easier to parse.
3. Loose coupling. When you just want to expose public APIs over the Internet REST is a good choice. REST is flexible on technologies using on both consumer and server side. 


## Summary
SOAP is useful in certain way. If you want to develope a banking system that require to high level of reliability then SOAP is the best choice. All the features of SOAP are required for banking system. 
