# sidebar_updater
A bot that will update reddit's sidebar
 
#usage  
sbup.help()     This prompt will be printed  
sbup.config()   parameters: ("user","pass", "subreddit","date")  
                subreddit and date are optional and default to  
                metalgearsolid and september 1st of this year.  
                The subreddit format does not include /r/ so  
                "metalgearsolid" is correct not "/r/metalgearsolid"  
                The date format is: "MM DD YYYY HH:MMXM" where the  
                ending "XM" is AM or PM.  
sbup.init()     No parameters, will create the first line at the  
                end of the sidebar. The exact action of this function  
                is to download the sidebar, add two spaces, a newline  
                and a GT symbol, and the "XXX days remaining. "  
sbup.update()   No parameters, will manually update the number once.  
sbup.run()      No parameters. Will call update at midnight every day  
                until the day count is less than 0.  
                
#todo
options for when to repeat (seconds hours days, a time)  
fix the "1 days left" issue  
display hours, minutes, seconds  
tweak idle behavior   
