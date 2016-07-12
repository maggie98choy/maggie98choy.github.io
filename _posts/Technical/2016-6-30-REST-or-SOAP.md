---
layout: post
title: REST vs SOAP
tags: 
- Web Services
- REST
- SOAP
published: false
categories:
- Technical
---

I've been developed several SOAP and REST web services applications in the past. I know pretty well of how to develop a 
web services application using either SOAP or REST approach. Recently, someone asked me why I choose this approach over 
another. It gave me a pause. So I did some homework and here is the summary of SOAP aand REST.

Let's tell a little background of both technologies before going into the reasons of choosing which approach for application.

### SOAP
SOAP(Simple Object Access Protocol) was developed by Microsoft for the purpose of replacing older web technologies DCOM 
(Distributed Component Object Model) and COBRA (Common Object Request Broker Architecture) that didn't work well on Internet.
SOAP is a mature web technology protocol that exposes individual operation as web services. It's rely exlusively on XML to define content of message. SOAP focuses on accessing name operation; each implement business logic through interfaces.

### REST
Many developers found cumbersome to develop code for SOAP. For example, develop SOAP web service using Javascript is required to write ton of code just to achieve simple task because we must create XML structure every time. REST is a light weight alternative to SOAP. Instead of relying on XML for exchanging message it uses URL approach. REST focuses on resource-based operation. It inherits CRUD (POST, GET, PUSH, DELETE) from HTTP operations. This make it easy for both developer and browser to consume public APIs as you have no control over on what's going on the consumer side. This is one of the main reason REST dominant nearly 70% of the market.

