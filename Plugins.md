# Follow this format to make your own plugin for HellBot.

```python3
"""
# def start(update, context):
    update.message.reply_text("Hello! Welcome to sukoongroup")
    
    def help(update, context):
        update.message.reply_text(
         """
        /start -> Welcome to the channel
        /help -> to get all command 
        /ban -> Reply or mention user id to ban
        /play -> Music Name or Youtube Link or Reply to Audio
        /unban -> Everyone can change messages
        /welcome ->  Set welcome message
        /goodbye -> Set goodbye message
        /quiet -> Disable "Sorry, only the person who..." & help messages
        /unquiet -> Enable "Sorry, only the person who..." & help messages
        /ping -> check my baby
        /kang -> steal the sticker hue hue
        /mstart -> start the music 
        /help -> help commands of music player 
        /mute -> shut the box of user 
        /vivi -> get user of information
        /afk -> Reason that make u afk
        /lang -> change language 
        /admins -> get all admin list
        /vivu -> contact owner
        /mimu -> contact co-owner 
        /adi -> contact dost
        /earnmoney -> join this channel https://t.me/Xpert366
        """
        )

        def content(update, context):
            update.message.reply_text(" We have all the commands available")

            def Start(update, context):
            update.message.reply_text("Add me to your group")

           def Help(update, context):
            update.message.reply_text("Add me to your group")

            def Start(update, context):
            update.message.reply_text("Add me to your group")

            dispatcher.add_handler(Telegram.ext.commandhandler('Start', Start ))
            dispatcher.add_handler(Telegram.ext.commandhandler('Help', Help ))

            updater.start_polling()
            updater.idle()
        
        Follow this format to make your own plugin for HellBot.

```python3
"""
A sample code to display hello without taking input.
"""
# this is a mandatory import
from . import *

# assigning command
@hell_cmd(pattern="hii$")
async def hi(event):
    # command body
    await eor(event, "Hello!")


# to display in help menu
CmdHelp("hii").add_command(
  "hii", None, "Says Hello!"
).add()
```

```python3
"""
A sample code to display hello with input.
"""
# this is a mandatory import
from . import *

# assigning command
@hell_cmd(pattern="hii(?:\s|$)([\s\S]*)")
async def hi(event):
    # command body
    _input = event.pattern_match.group(1)
    if _input:
        await eor(event, f"Hello! {_input}")
    else:
        await eor(event, "Hello!")


# to display in help menu
CmdHelp("hii").add_command(
    "hii", "<text>", "Display Hello with a input!"
).add()
```


## To get more functions read codes in repo.A sample code to display hello without taking input.
"""
# this is a mandatory import
from . import *

# assigning command
@hell_cmd(pattern="hii$")
async def hi(event):
    # command body
    await eor(event, "Hello!")


# to display in help menu
CmdHelp("hii").add_command(
  "hii", None, "Says Hello!"
).add()
```

```python3
"""
A sample code to display hello with input.
"""
# this is a mandatory import
from . import *

# assigning command
@hell_cmd(pattern="hii(?:\s|$)([\s\S]*)")
async def hi(event):
    # command body
    _input = event.pattern_match.group(1)
    if _input:
        await eor(event, f"Hello! {_input}")
    else:
        await eor(event, "Hello!")


# to display in help menu
CmdHelp("hii").add_command(
    "hii", "<text>", "Display Hello with a input!"
).add()
```


## To get more functions read codes in repo.
