# The Bob Toolkit: Universal Charm Framework Manager

Welcome to the Bob Toolkit, your one-stop-shop for managing 
your [Charm Framework](https://github.com/neoground/charm) projects like a pro! 
With just a few keystrokes, Bob can help you create new projects
and access console commands of your projects easily. 

In a galaxy not so far away, Bob (short for Binary Operations Butler) 
was created to serve as the ultimate command-line companion for 
Charm Framework developers. Bob needs PHP 8.0 or above.
It's so easy to use, even a Wookiee could do it!

Requirements:

- PHP 8.0 or above
- Composer available in `PATH`


## Getting Started

To begin your epic journey with Bob, just follow these simple steps:

1. Ensure that you have PHP 8.0 or above and Composer installed and available in your system's `PATH`.
2. Download `bob` and make `bob` executable:
    ```sh
   curl -fSsL -o bob https://raw.githubusercontent.com/neoground/charm-toolkit/main/bob && chmod +x bob
    ```
   If `curl` is not available on your system, you can also download it with `wget`:
   ```sh
   wget -O bob https://raw.githubusercontent.com/neoground/charm-toolkit/main/bob && chmod +x bob
    ```
3. To use bob globally, move it to `/usr/local/bin/`, which should be in your system's `PATH`.
    ```sh
   sudo mv bob /usr/local/bin/
    ```
4. Execute `bob` from your terminal and watch the magic happen!


## Goals of this toolkit

Our mission is to make the Bob Toolkit the ultimate CLI tool for the Charm Framework, 
providing easy support for all the command-line tasks you'll encounter in your projects. 
We aim to create a powerful and user-friendly interface that integrates seamlessly 
into any system, much like how C-3PO's fluency in over six million forms of communication 
makes him the perfect protocol droid.

With the Bob Toolkit, we're not only making it easier to manage your Charm projects 
but also providing you with a faithful companion for your journey through the 
galaxy of web development. Together, we'll forge a path to bring balance to the 
Force and help you conquer even the most challenging coding challenges.

So, strap in and prepare for lightspeed as we embark on this adventure with 
the Bob Toolkit, making your Charm Framework experience out-of-this-world!


## Examples

### Create a new project

Bob can create new Charm projects faster than a warp-speed 
Millennium Falcon! To create a new project called `holoarchive` in a 
subdirectory named `holoarchive`, simply run:

```sh
bob new holoarchive
```

Bob will generate all the necessary files and folders for your 
shiny new `holoarchive` project, and you'll be ready to code in no time.

### Accessing console commands

Bob is like the trusty astromech droid R2-D2, always ready to provide 
assistance and perform vital tasks. To access the console commands 
for your Charm projects, just navigate to the project directory and run:

```sh
bob command [arguments] [options]
```

Bob will execute the specified command, using any provided arguments 
and options, making it easy to manage your Charm project with just 
a few beeps and boops.

For example, to run the cron jobs for your project, simply execute:

```sh
bob cron:run
```

Bob will take care of running the scheduled tasks, 
just like R2-D2 maintaining the systems of an X-Wing fighter.

### Development Server

The `bob` command-line tool offers an incredibly convenient development server 
that allows you to quickly run and test your Charm applications. 
By default, the server is set to run on `localhost` and listens to port `8000`.
In this section, we'll explore how to use `bob serve` with different parameters to meet your development needs.

This development server is based on PHP's [built-in web server](https://www.php.net/manual/en/features.commandline.webserver.php).

#### Starting the Development Server

To start the development server with default settings, simply navigate to your
Charm project's root directory and execute the following command:

```sh
bob serve
```

This will launch the server on `localhost:8000`. You can now open your favorite browser and visit 
`http://localhost:8000` to interact with your application.

#### Custom host and port

To specify a custom host, run the following command:

```sh
bob serve 192.168.0.2
```

This will start the server on the `192.168.0.2` IP address and the default port `8000`.
Use `0.0.0.0` to listen on all interfaces.

To specify a custom port, run the following command:

```sh
bob serve localhost 9000
```

This will start the server on `localhost` with a custom port `9000`.

To specify both a custom host and port, run the following command:

```sh
bob serve 10.0.0.2 9000
```

This will start the server on the `10.0.0.2` IP address and the custom port `9000`.

### Self-update

In a galaxy far, far away, tools need to stay up to date
to support the Rebellion's cause. That's why Bob comes 
with a built-in self-update feature. This handy function ensures 
your toolkit remains in sync with the latest developments 
and improvements, just like a well-maintained hyperdrive system.

To access this self-update functionality, simply execute the following command:

```sh
bob self-update
```

Keep in mind that this command should only be used when Bob is 
installed at `/usr/local/bin/bob`. This is the default location 
for most installations, and the self-update feature is designed 
to work seamlessly with it.

When executed, the self-update command fetches the latest version 
of the Bob script from the Charm Framework repository, 
ensuring you're always equipped with the most recent tools and fixes. 
This way, you can continue your quest to build exceptional 
web applications and help the Rebellion triumph against the
dark forces of outdated code and inefficient tools.

Remember, a well-updated toolkit is a powerful ally. 
Stay sharp and may the Force be with you!


## Conclusion

Bob is the ultimate toolkit for Charm Framework developers, 
offering a powerful and intuitive way to create and manage projects. 
With Bob by your side, you'll be the Jedi Master of Charm Framework, 
wielding your coding powers with the grace and wisdom of Yoda himself.

So, what are you waiting for? Get started with Bob today, 
and may the Force be with you on your Charm Framework journey!
