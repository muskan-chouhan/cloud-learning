### useradd

Creates a new Linux user.

Syntax:

```bash
sudo useradd username
```
sudo useradd -m testuser          //create automatically home directory
Example:

```bash
sudo useradd rahul
```

Check user:

```bash
id rahul
```

When to use:

Create a new user account on a Linux server.

Real World Example:

A new employee joins the company and needs server access.



### passwd

Sets or changes the password of a Linux user.

Syntax:

```bash
sudo passwd username
```

Example:

```bash
sudo passwd testuser
```

When to use:

- Set password for a new user.
- Change an existing user's password.

Difference:

- `useradd` → Creates a user.
- `passwd` → Sets or changes the user's password.


### usermod

Modifies an existing user account.

Syntax:

```bash
sudo usermod -aG group_name username
```

Example:

```bash
sudo usermod -aG sudo rahul
```

Options:

- `-a` → Append (keep existing groups)
- `-G` → Add user to a group

Check:

```bash
groups rahul
```

When to use:

Add an existing user to a new group.

Real World Example:

Give a developer sudo access after promotion.




### userdel

Deletes a Linux user.

Syntax:

```bash
sudo userdel username
```

Delete user with home directory:

```bash
sudo userdel -r username
```

Example:

```bash
sudo userdel -r testuser
```

Options:

- `-r` → Remove user's home directory.

Real World Example:

Delete the account of an employee who has left the company.