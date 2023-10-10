# AirBnB-clone Web-dynamic

Resources

- [Selector](https://intranet.alxswe.com/rltoken/Bl2mJVVG07XCP6E8qtsQMg)
- [Get and set content](https://intranet.alxswe.com/rltoken/oM3b0a0FGTy6AQ_UJ201Yw)
- [Manipulate CSS classes](https://intranet.alxswe.com/rltoken/LL2uScQvjWnj2ZEx2CzxXw)
- [Manipulate DOM elements](https://intranet.alxswe.com/rltoken/6JtTz9SaNX3AyVXht4tMYA)
- [Document ready](https://intranet.alxswe.com/rltoken/1AbzN1nEfBKoSjB-9kjmrA)
- [Introduction](https://intranet.alxswe.com/rltoken/OGDoIOd0cdmwDJFJy4aw5w)
- [GET & POST request](https://intranet.alxswe.com/rltoken/kmBzs_QPD72Oz--Yk80JHw)
- [HTTP access control (CORS)](https://intranet.alxswe.com/rltoken/tzqJx5SS5cF1BW_lAnXqqg)

## Import JQuery
```
<head>
    <script src="https://code.jquery.com/jquery-3.2.1.min.js"></script>
</head>
```

## Before starting the project…

You will work on a codebase using [Flasgger](https://intranet.alxswe.com/rltoken/VmGDpw_DCN16OJt_UoqsDQ), you will need to install it locally first before starting the RestAPI:

```
$ sudo apt-get install -y python3-lxml
$ sudo pip3 install flask_cors # if it was not installed yet
$ sudo pip3 install flasgger
```

If the RestAPI is not starting, please read the error message. Based on the(ses) error message(s), you will have to troubleshoot potential dependencies issues.

Here some solutions:

`jsonschema` exception

```
$ sudo pip3 uninstall -y jsonschema
$ sudo pip3 install jsonschema==3.0.1
```

`No module named 'pathlib2'`

```
$ sudo pip3 install pathlib2
```
### Expose ports from your Vagrant

In your Vagrantfile, add this line for each port forwarded

```
# I expose the port 5001 of my vm to the port 5001 on my computer
config.vm.network :forwarded_port, guest: 5001, host: 5001
```

if you need to expose other ports, same line but you will need to replace the “guest port” (inside your vagrant) and your “host port” (outside your vagrant, used from your browser for example)

It’s important in your project, to use the AirBnB API with the port 5001

# Tasks

#### 0. Last clone!

A new codebase again? Yes!

For this project you will fork this [codebase](https://intranet.alxswe.com/rltoken/18CpThAKqBP5uviO1DSSGw):

- Update the repository name to AirBnB_clone_v4
- Update the README.md:
    - Add yourself as an author of the project
    - Add new information about your new contribution
    - Make it better!
- If you’re the owner of this codebase, create a new repository called AirBnB_clone_v4 and copy over all files from AirBnB_clone_v3
- If you didn’t install Flasgger from the previous project, it’s time! `sudo pip3 install flasgger`

**Repo:**

- GitHub repository: `AirBnB_clone_v4`
