### Practice SQL queries with Python and sqlite3

You are using databases all the time, though you might not realize it. Even if you have never even queried a table, you almost certainly own a device which runs applications that use a lightweight database engine. By far the most widely used database engine is [SQLite](https://sqlite.org/index.html). It is so nearly ubiquitous that almost every mobile phone and web browser use it.

Are you a Python programmer, but not really proficient in SQL? You're in luck, because Python, adhering to it's philosophy of "batteries included", has [support for SQLite built-in](https://docs.python.org/3/library/sqlite3.html)!

"Ah, but wait", I hear you saying, "does SQLite use the standard SQL languge?" The answer is yes..., well mostly anyway. "SQLite understands most of the standard SQL language. But it does omit some features while at the same time adding a few features of its own." If interested, read [SQL As Understood By SQLite](https://sqlite.org/lang.html). In short, if you learn SQL using SQLite, then you will be able to interact with most any other database engine that supports standard SQL.

Below we'll go through some practical exercises with a simple dataset. I'll assume that the reader has intermediate Python skill but has little knowledge of SQL. We'll see how to create a database from a CSV file, and then how to add another table. We'll learn how to do queries, from simple ones to more complex ones.

Using sqlite3 from Python liberates me from the pain of setting-up and maintaining a client/server SQL database engine such as MySQL, or PostgreSQL. SQLite has a command-line interface, however since most data scientists will want to do further analysis on their query results, it makes sense to learn it from within the context of the Python interpreter. Whether you are just learning SQL and want to practice for that Data Scientist interview, or whether you have SQL experience and just want to see if sqlite3 has what you require, I hope you'll find these examples helpful.

__[CLICK HERE TO BEGIN USING THE NOTEBOOK]('./StarForceAnalysis.ipynb').__