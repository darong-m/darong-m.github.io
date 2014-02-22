---
layout: post
title: "Design by Contract"
date: 2014-02-22 23:49:37 +0700
comments: true
categories: [design by contract]
---

Note on some basic ideas with Design  by Contract principle.

<!-- more -->

# Definition

- **Software System** : A software system is a set of mechanisms to create, access, and change collections of information called objcts.
- **Object** : An object is a software machine allowing programs to access and modify a collections of data.
- **Feature** : An operation that programs may apply to an object.
- **Command** : A feature that may change an object; It changes the visible properties of the object through queries.
- **Query** : A feature that accesses an object.

- **Instruction** : An instruction denotes a basic operation to be performed during the program's execution.
- **Expression** : An expression denotes a value used by instruction for its execution.
- **Syntax** : The syntax of a program is the structure and forms of its text.
- **Semantics** : The semantics of a program is the set of properties of its potential executions.

- **Client** : A client of a software mechanism is a system of any kind, such as a software element, a non-software system, or a human user, that uses it. For its clients, the mechanism is a **supplier** .
- **Interface** : An interface of a set of software mechanisms is the description of techniques enabling clients to use these mechanisms.

- **Class** : A class is the description of a set of possible run-time objects to which the same features are applicable.
Classes are static and objects are dynamic.

- **Contract** : A contract is a specification of properties of a software element that affect its use by potential clients.

- **Information Hiding** : Information hiding is the mechanism separating interface information from implementation details, and enabling clients to use routines and other software elements on the basis of the interface only.

# Concept

Finding appropriate classes is a central part of the task of of software **design**, devoting to organizing the essential **structure**, or **architecture**, of a program as opposed to writing down the details, or **implementation**.

To find good classess, we search the problem domain for concepts that:

- describe sets of objects(their future instances).
- can be explained clearly.
- can be characterized in terms of clearly defined *features*, including both queries and commands, applicable to the corresponding objects.

A client calling a feature must make sure that the **precondition** holds before the call.
A feature must make sure that if its precondition held at the beginning of its execution, its **postcondition** will hold at the end.
A **clas invariant** must hold as soon as an object is created, then before and after execution of any of the class features available to clients.
