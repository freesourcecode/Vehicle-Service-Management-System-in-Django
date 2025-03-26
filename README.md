# Vehicle Service Management System in Django with Source Code

The **Vehicle Service Management System Project in Django** created based on **Python**, **Django**, and **SQLITE3 Database**.

The admin side and the user side are both included in a Vehicle Management System project.

The administrator has complete authority over all car requests and can determine whether or not they can be granted.

They can make changes to the driver and vehicle lists, as well as add new drivers and vehicles.

From the admin interface, an admin may oversee the entire booking process, such as which car to assign to a specific user and which driver to dispatch.

> [!NOTE]
> To start creating a **Vehicle Service Management System Project in Python Django**, makes sure that you have PyCharm Professional IDE Installed in your computer.

## Admin Features:

* The administrator will log in (execute the following command in cmd to get the username and password).
* Your admin account will be established after you enter your username, email, and password.
* On the dashboard, the admin may see how many customers, mechanics, and recent service orders there are after logging in.
* Each customer invoice is visible to the administrator (if two request made by same customer it will show total sum of both request)
* Admins have access to the company and can see, add, update, and delete them.
* Admin can approve (hire) technicians depending on their skills (as asked by the mechanic).
* The Admin can view, alter, and delete service requests/enquiries received by customers.
* Admin can also submit service requests (assuming the customer has arrived at the service center/office).
* Admin can authorize a customer’s request for service, assign it to a mechanic for repair, and provide a cost based on the problem description.
* The Admin can see all of the request’s service costs (both approved and pending)
* Customer/company feedback can be viewed by the administrator.

## Customer Features

* Customers will register and log in to the system, where they will be able to request servicing for their vehicle by giving information (vehicle number, model, problem description etc.).
* If the client changes their mind or the request is not allowed by the admin, the customer can check the pricing and progress of the service. If the customer changes their mind or the request is not approved by the admin, the customer can delete the request (enquiry).
* Customer can see/edit their profile and check the status of their Request(Enquiry), which can be Pending, Approved, Repairing, Repairing Done, or Released.
* Customer can also check invoice information or repaired vehicles.


## How to Create a Project Vehicle Service Management System in Django?
Here are the steps on how to create a **Django Vehicle Service Management System** with Source Code.

1. **Open file**.

First, open "pycharm professional" after that click "file" and click "new project".

2. **Choose Django**.

Next, after click "new project", choose "Django" and click.

3. **Select file location**.

Then, select a file location wherever you want.

4. **Create application name**.

After that, name your application.

5. **Click create**.

Finish creating project by clicking “create” button.

6. **Start Coding**.

Finally, we will now start adding functionality to our Django Framework by adding some functional codes.

## Functionality and Codes of the Vehicle Service Management System Project in Django with Source Code

### Create template for the add customer form in Vehicle Service Management System in Django.

In this section, we will learn on how create a templates for the add customer form. 
To start with, add the following code in your admin_add_customer.html under the folder of /templates/.

```{% extends 'vehicle/adminbase.html' %}
{% load widget_tweaks %}
{% block content %}
<head>
  <style media="screen">
    input[type=text], select,input[type=number] ,input[type=password], textarea{
    width: 100%;
    padding: 12px 20px;
    margin: 8px 0;
    display: inline-block;
    border: 1px solid #ccc;
    border-radius: 4px;
    box-sizing: border-box;
  }

  input[type=submit] {
    width: 100%;
    background-color: #4CAF50;
    color: white;
    padding: 14px 20px;
    margin: 8px 0;
    border: none;
    border-radius: 4px;
    cursor: pointer;
  }

  input[type=submit]:hover {
    background-color: #45a049;
  }


  </style>


</head>

<br><br><br><br><br>
<h3 style="text-align:center;">CREATE CUSTOMER ACCOUNT</h3>
<div>
  <form method="post"  enctype="multipart/form-data"  style="margin-left:200px;margin-right:200px;">
      {% csrf_token %}

        <label for="first_name">First Name</label>
        {% render_field userForm.first_name class="form-control" placeholder="First Name" %}
        <label for="last_name">Last Name</label>
        {% render_field userForm.last_name class="form-control" placeholder="Last Name" %}
        <label for="mobile">Mobile</label>
        {% render_field customerForm.mobile class="form-control" placeholder="Mobile" %}
        <label for="address">Address</label>
        {% render_field customerForm.address class="form-control" placeholder="Address" %}
        <label for="username">Username</label>
        {% render_field userForm.username class="form-control" placeholder="Username" %}
        <label for="password">Password</label>
        {% render_field userForm.password class="form-control" placeholder="Password" %} <br><br>
        <label for="profile_pic">Profile Picture</label>
        {% render_field customerForm.profile_pic class="form-control" placeholder="Profile Picture" %}

    <input type="submit" value="Create">
  </form>
</div>



<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
{% endblock content %}
```

### 📌 Here's the full documentation for the [Vehicle Service Management System in Django](https://itsourcecode.com/free-projects/python-projects/vehicle-service-management-system-project-in-django-with-source-code/)



