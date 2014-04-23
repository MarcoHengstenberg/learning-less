# Who is this JSON anyways?

After I talked on length about all the things we will do, let's finally *do* something. Shall we?

## package.json

Like any good person with the last name of .json, our `package.json` is easy to write, read and be interpreted by a computer or human being.

Just make sure to write the projectname in one word, no spaces, no special characters – dashes are allowed and end all your lines inside the brackets with a comma.

**Again:** Always make sure to end lines with a comma or you will soon go through endless lines of code, searching for the missing one.

So without any further introduction here the first lines of code.

### Project Metadata

```
{
  "name" : "ProjectName",
  "version" : "0.0.1",
  "description": "Description of the project",
  "author" : "Your Name",
}
```

This is basic metadata for your project and there is much more you could add (there is also a [spec](https://www.npmjs.org/doc/json.html) if you are into that sort of thing). The minimum should be the name of the project and the version you are working on. Always make sure to end lines... wait, I told you that already.

You could add keywords, contributors, a license, a URL, a repository with or without issues and whatnot. Again, if you are into that sort of thing, simply follow the link to the specification and you will find all metadata glory with examples. As you will see, one can get quite [crazy](http://registry.npmjs.org/npm/latest) with this.

### devDependencies

Metadata doesn't do much apart from telling humans or computers what to expect or make out of something else. Now, we are writing the 'something else' part. As we want to work with Grunt, we are going to write that down:

```
{
  "name" : "ProjectName",
  "version" : "0.0.1",
  "description": "Description of the project",
  "author" : "Your Name",

  "devDependencies" : {
    "grunt" : "~0.4.0",
  }
}
```

We are telling the program that we work with Grunt. Yes, it is that easy. Let's add some of the tasks we want to work with:

```
{
  "name" : "Projectname",
  "version" : "0.1.0",
  "description": "Description of the project",
  "author" : "Marco Kunz",
  "private" : "true",

  "devDependencies" : {
    "grunt" : "~0.4.0",
    "grunt-htmlhint": "*",
    "grunt-contrib-less" : "*",
    "grunt-autoprefixer" : "*",
    "grunt-contrib-cssmin" : "*",
    "grunt-contrib-watch" : "*",
    "matchdep" : "*"
  }
}
```

That's it. You just created the package.json file. It will always follow the same pattern and as long as you watch for your syntax, there won't be much trouble with it.

The best thing about it is its reusability. You can simply copypasta it into any project directory, change the metadata, keep the tasks and it will still work. Adding tasks or changing them is not a problem.

Now, you might be thinking:"Tasks, he said." Yes, I did. I will explain what the above mentioned tasks are good for in the next step.