Trying netlify & git lfs

Doing this:
* https://docs.netlify.com/large-media/requirements-and-limitations/#requirements
* https://docs.netlify.com/large-media/setup/#configure-file-tracking
* https://www.netlifycms.org/docs/netlify-large-media/

```
netlify plugins:install netlify-lm-plugin
netlify lm:install
```

```
netlify link
netlify lm:setup
```

Say what to track with git lfs:
```
git lfs track "public/image"
```

> After running these commands, you will be presented with a custom command to run in order to use Netlify Large Media in your shell. Copy and run this command.

```
 Run this command to use Netlify Large Media in your current shell   
                                                                    
           source /Users/nick/.netlify/helper/path.bash.inc   
```

> Uploading tracked files to the Netlify Large Media storage service requires Git to have access to the /.netlify/large-media path on the connected site. 

> Continue working in your repository as normal. Any files you add or change which match your tracking rules will automatically be handled by Git LFS and Netlify Large Media on every pushed commit.

It works! hurray

* [the public foler](https://www.netlifycms.org/docs/configuration-options/#media-and-public-folders)
* [CMS with lfs](https://docs.netlify.com/large-media/overview/#large-media-docs)
* [git setup](https://docs.netlify.com/large-media/setup/#configure-file-tracking)
* https://www.atlassian.com/git/tutorials/git-lfs


