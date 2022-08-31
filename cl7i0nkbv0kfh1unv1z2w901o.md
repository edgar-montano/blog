## How to list all the commands available in package.json

# Where art thou commands?

When first creating a project using a bundler like *create-react-app* you might quickly forget the list of commands or scripts you can run using npm. 

The solution to this is usually just briefly glancing at the **package.json** file in the root directory of your project, and locating the `"scripts"` section to show which scripts are defined for your project. 


![package.json.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1661895811991/6qmTAio3h.png align="left")

As you can see we have the following commands available to us:
- *start*
- *build*
- *test*
- *eject*

From here we can simply use *npm run <command>* to execute the command we desire. For instance, `npm run start` will run the *start* script. 

Unfortunately, this solution can be somewhat tedious, especially if you are dealing with a large and complex application where the **package.json** is significantly larger. 

# Solution `npm run`


![oh wow excuse me gif.gif](https://cdn.hashnode.com/res/hashnode/image/upload/v1661897108670/MI3Y_oXWL.gif align="center")


*Yep. That simple. Seriously.* 

Simply use `npm run` without any additional parameters and you will see all the scripts included in your **package.json.** 


![npm-run.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1661897304524/FqFd3-_DV.png align="left")

In addition to giving us information about what scripts we can run, it also provides a bit of insight into the scripts which is actually very useful information we can use later on without constantly consulting the **package.json** file. 

According to the docs:
> This runs an arbitrary command from a package's "scripts" object. If no "command" is provided, it will list the available scripts.

> `run[-script]` is used by the test, start, restart, and stop commands, but can be called directly, as well. When the scripts in the package are printed out, they're separated into lifecycle (test, start, restart) and directly-run scripts.

I highly recommend you take a glance at the [npm-run-script docs](https://docs.npmjs.com/cli/v8/commands/npm-run-script) for more info.

## `npm help run`

If you are curious about the documentation and want to learn more, I encourage you to run `npm help run`. It'll redirect you to the most current documentation. 

