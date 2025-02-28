```
CREATE DATABASE my_database;
USE my_database;
```

```
CREATE TABLE employees (
    id INT AUTO_INCREMENT PRIMARY KEY,  -- Unique ID for each employee
    name VARCHAR(255) NOT NULL,         -- Employee name (max 255 characters)
    department VARCHAR(255),            -- Department name
    salary DECIMAL(10, 2)               -- Salary with 2 decimal points
);
```

<table>
        <tr>
            <th>ID</th>
            <th>Name</th>
            <th>Department</th>
            <th>Salary</th>
        </tr>
 
</table>

```

INSERT INTO employees (name, department, salary) 
VALUES ('John Doe', 'HR', 50000.50);
('Alice Smith', 'Sales', 60000),
('Bob Johnson', 'IT', 70000),
('Charlie Brown', 'Finance', 55000);

```

<table>
        <tr>
            <th>ID</th>
            <th>Name</th>
            <th>Department</th>
            <th>Salary</th>
        </tr>
        <tr>
            <td>1</td>
            <td>John Doe</td>
            <td>HR</td>
            <td>50000.50</td>
        </tr>
        <tr>
            <td>2</td>
            <td>Alice Smith</td>
            <td>Sales</td>
            <td>60000.00</td>
        </tr>
        <tr>
            <td>3</td>
            <td>Bob Johnson</td>
            <td>IT</td>
            <td>70000.00</td>
        </tr>
        <tr>
            <td>4</td>
            <td>Charlie Brown</td>
            <td>Finance</td>
            <td>55000.00</td>
        </tr>
</table>


    
