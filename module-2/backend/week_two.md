## Week Two - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON - YOU are a web developer!!!).

Note: When you're done, submit a PR.

1. At a high level, what is ActiveRecord? What does it do/allow you to do?
ActiveRecord is a database management tool that creates relationships between models.
2. What kind of methods are `belongs_to`, and `has_many`? (i.e. class or instance) Give an example.
Class methods. An item `belongs_to` a merchant, and a merchant `has_many` items.
3. What do they allow you to do?
They allow you to call `item.merchant` and `merchant.items`
4. What's the difference between agile workflow and waterfall method?
Agile is about breaking the functionality into pieces and tackling design, testing, deployment all at once for these features whereas waterfall requires planning the project out ahead of time and handling each step of the process for the whole project in order.
5. What is the difference between `#new` and `#create`?
`create` makes a new instance and saves it while `new` does not save it to the database
6. At a basic level, what does cURL allow you to do?
Peek into the Whois information for a site
7. In a database that's holding students and teachers, what will be the relationship between students and teachers? Draw the schema diagram.
a student `has_many` teachers and a teacher `has_many` students. They would probably be linked by another table called enrollments that would keep track of teacher-student relationships through foreign keys to both tables.

STUDENTS
id name
1   Joe

TEACHERS
id - name
1   Mr. Joe

ENROLLMENTS
id  - student_id - teacher_id
1     1            1

8. Define foreign key, primary key, and schema.
a foreign key links a column from one table to the primary key from another table.
a primary key is an independent column in a table that other columns relate to.
a schema is a blueprint for creating a database.
9. Describe the relationship between a foreign key on one table and a primary key on another table.
A foreign key column in one table is the primary key column of another table.
10. What are the parts of an HTTP response?
status/headers/body
status: hopefully 200 OK
headers: dates, connection, server information
body: html
11. Describe some techniques to make our Sinatra code more DRY. Give an example of when you would use these techniques.
Partials! for forms, navigation, footers


### Optional Questions

1. Name your five favorite ActiveRecord methods (i.e. methods your models inherit from ActiveRecord) and describe what they do.
2. Name your three favorite ActiveRecord rake tasks and describe what they do.
4. What can you expect from a group as you begin working together? As you continue working together?
5. What two columns does `t.timestamps null: false` create in our database?
6. What cURL flag can you use to send a `POST` request?
7. What case does JSON (and JavaScript) use for multi-word variables?
8. What case does Ruby use for multi-word variables?
9. In a database that's holding schools and teachers, what will be the relationship between schools and teachers?
10. In the same database, what will you need to do to create this relationship (draw a schema diagram)?
11. Give an example of when you might want to store information besides ids on a join table.
12. Describe and diagram the relationship between patients and doctors.
13. Describe and diagram the relationship between museums and original_paintings.
14. What are some examples of acceptable values for the parts of an HTTP response?
15. What types of output do we want to test when we test our controllers?
16. What could you see in your code that would make you think you might want to create a partial?
17. Why might you use a helper method?
