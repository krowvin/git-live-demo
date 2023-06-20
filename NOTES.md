# Workshop Notes
*Today's workshop is going to show a lot of python, cwms, specified **location levels**, and even some cwms vue.*

## The workshop focuses on using git and github 
    However, we need content to really drive home the use cases of version control! 

### What/How
What is a **"Specified Location Level"**?   
  From the great Rachel Felice, PE  
  A Specified Location level is:
> Location levels are lake water elevations defined by water control manuals at each lake to denote inactive pool, conservation pool, flood pool, surcharge pool (if applicable) and max pool. 
Location levels can also be defined for specific streamgages per district regulation or NWS. These levels note regulating stages or flood stages.

Today I plan to create a python script that pulls specified location level data from CDA and stores it into
JSON files to assist with load times and reduce the number of requests. This is not a true cache, 
and still requires disk IO. It helps to have it stored locally on your disk! 

In the cloud
you would use something like Redis, MemCacheD, or even a language specific cache to store frequently
requested data. This gives you full control over when something should be updated!

### When
You could then use the JSON files locally (and frequently) to pull level
data for client/server-side applications either on the browser (javascript) or in other apps/scripts (python/java/etc). Updating daily, or even every hour if you update your levels often!

### Why
The reason you may want to do this is because you can run this python caching script once a day 
(or more) and only update your json files when needed.  

This will reduce load on CDA, and lower the wait time for large sets of level data. 

If you update levels often, you would want to update this script too. 

### Alternative - Normal Method
And of course, if it suits your applications and you only need 1 or 2 levels you could pull the 
data in parallel directly from your client. 


Share link to github page that has instructions for git/github

**share screen, walk through README.md instructions**
Good news everyone! No slides today!



# Project Outline
  * Imports
  * Constants
  * Get data function (from CDA)
  * save function (stores to JSON)
  * if __name__ == "__main__": entry point for our program. Ensures this is only called if this script is ran directly (not part of a class)
  * 
## Steps and when to commit (for workshop)
1. Initial project (readme/ignore) - init
2. Second commit, project structure. Directories, main.py, workspace. Add comments about the parts of our code (pseudo code)
1. Create branch to work on data - data-fetch-store
	3.1 First branch commit, write & tested getLevelData function
	3.2 Second branch commit, write & tested save function
2. Merge branch into main
3. Create a branch for our html - could also be a new REPO if either is big enough of a project!
	If it's just you, it's really only for your use
	new web branch can contain your frontend code, and the other branch your backend
	this new web branch could be a github pages webpage
4. Write HTM
	6.1 init for html in new branch
	6.2 Write html and javascript to read json -> Test it! -> COmmit
	6.3 Add styling to the page, test it, commit!
5. Show how to add someone to your repo
6. Show how they could create a branch to work on their code, exaplain why you might fork instead

# Deployment
This is great and all, now where do I deploy my python script?  

You can place it on the webserver itself (recommended) or you can run it on your T7 or local windows
servers and push via SFTP to your public webserver.  

Example crontab line on our public RHEL webserver  
```cron
# Update the level cache once a day from CWMS Data API
5 8 * * * <path_to_user_dir>/bin/FetchLocationLevels.sh >/dev/null 2>&1>/dev/null 2>&1
```
(GMT) -> Ran early morning before work day



