SOLID :-

S - Single Risponsiblity Principle
O - Open Closed Principle
L - Liskove principle
I - Interface Segrigation
D - Dependency Injection

-------------------------------------------------

1. SRP :-
           Single Responsiblity principle describes that one method should responsible for only one task not multiple.

   Let say we have a different type of bird and each bird can make different type of sound and bird can fly or not, for that we created a method in that we are managing different birds and
   its functionallity and it breaks the SPR rule because one method can resposible for one type of operation.

   Here to many if else or to many operation in one method will cause so many problem. we have to write test case for each if-else and merge conflict might occur if two developers are working on same method but on
   different feature. Modularity and readiblity will not be present if it voilates SRP.

   SRP said each functionallity should have sperate implementaion either it should be a separte class of function.

2. OCP :-
           Open Closed Principle says that Method or class is open for updating or modify existing implementation but close for adding new feature.
           Because New feature can break the existing feature it might cause regression failure to avaiod this create a new class and implement functionallity.
   https://airlock-on-edge.woolf.university/?url=https%3A%2F%2Fscaler-production-new.s3.ap-southeast-1.amazonaws.com%2Fattachments%2Fattachments%2F000%2F044%2F102%2Foriginal%2FNote_21_May_2023.pdf%3FX-Amz-Algorithm%3DAWS4-HMAC-SHA256%26X-Amz-Credential%3DAKIAIDNNIRGHAQUQRWYA%252F20250831%252Fap-southeast-1%252Fs3%252Faws4_request%26X-Amz-Date%3D20250831T122023Z%26X-Amz-Expires%3D561600%26X-Amz-SignedHeaders%3Dhost%26X-Amz-Signature%3Da72c26cac45141d21afa401a63dd6d414e45464c2ef1ad13e1810e486ec1a211&resourceId=2c030a9e-fffe-40f7-ae9c-9156ec4d016a&studentId=6d8b3c33-5eca-4179-be82-46270b32db45&token=eyJhbGciOiJIUzI1NiJ9.eyJpZCI6IjZkOGIzYzMzLTVlY2EtNDE3OS1iZTgyLTQ2MjcwYjMyZGI0NSIsImlzcyI6InVybjpXb29sZlVuaXZlcnNpdHk6c2VydmVyL3NlcnZpY2UvYWNjZXNzIiwiaXNWZXJpZmllZCI6dHJ1ZSwia2luZCI6Im9hdXRoIiwib3JnIjp7Imdyb3VwcyI6W10sImlkIjoiOWIxN2Y1Y2UtMTA3OC00ZmRmLWFlYzAtMDJiZjRlY2ZiMGE2In0sInNjb3BlIjoiKiJ9.aFsteoGqlMosCRJku7qmGZuq61DO52WXIBl2Adojnb8
