# Data :-

    Any information which is useful for our requirement.

# Database :-

    Database is way in DBMS which help's to manage data in different forms depends on the type of DBMS. we can mangae data in form of tables, JSON etc.

# DBMS :-

    Database Mangaement system is a software that manges the multiple databases together. Their is different DBMS provides like.

    1. MySql :- Relational database
    2. Sql Server :- Relational database
    3. Oracle :- Relational database
    4. MongoDB :- Store Data in JSON
    5. Redis :- Store data in Key Value pair

    Many DBMS providers are their in market it depends on our use case which we want to use.

# Relation :-

    Relation is define information related to something suppose student is one relation

# Atrributes :-

    Properties of Relation or we can say column in entity or table.

# Degree :-

    Number of Coulmns in Table.

# Cardinality :-

    Number of Rows in table

# Tuples :-

    Rows or recors in table.

# Keys :-

    Collection of Attributes or Just Attribute which helps in uniqely identifing the touple.

# Super Key :-

    It same defination of keys.

# Candidate Key :-

    Collection of unnecessary Attributes or Just Attribute which helps in uniquely identifing the topule.

    All Candidate key is super key but not all super key is candidate key.

# Composite Key :-

    Collection of Attributes or more than one attribute which helps in uniqely identifing the touple.

    All Composite key is super key but not all super key is Composite key.

# Example :-

    Students table has FirstName, LastName, PhoneNo, Email

    Attribute Collection                        SuperKey        CandidateKey        CompositeKey

    FirstName                                   ❌              ❌                  ❌
    LastName                                    ❌              ❌                  ❌
    FirstName,LastName                          ❌              ❌                  ❌
    FirstName,PhoneNo                           ✅              ❌                  ✅
    LastName, PhoneNo                           ✅              ❌                  ✅
    FirstName,Email                             ✅              ❌                  ✅
    LastName, Email                             ✅              ❌                  ✅
    FirstName, LastName, PhoneNo                ✅              ❌                  ✅
    PhoneNo                                     ✅              ✅                  ❌
    Email                                       ✅              ✅                  ❌
    PhoneNo, Email                              ✅              ❌                  ✅
    FirstName, LastName, PhoneNo, Email         ✅              ❌                  ✅

