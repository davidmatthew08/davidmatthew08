local Rayfield = loadstring(game:HttpGet('https://sirius.menu/rayfield'))()

local Window = Rayfield:CreateWindow({
   Name = "beat up bloxian script",
   LoadingTitle = "plss wait",
   LoadingSubtitle = "by david",
   ConfigurationSaving = {
      Enabled = false,
      FolderName = nil, -- Create a custom folder for your hub/game
      FileName = "beat up bloxian"
   },
   Discord = {
      Enabled = false,
      Invite = "link in description", -- The Discord invite code, do not include discord.gg/. E.g. discord.gg/ABCD would be ABCD
      RememberJoins = true -- Set this to false to make them join the discord every time they load it up
   },
   KeySystem = true, -- Set this to true to use our key system
   KeySettings = {
      Title = "beat up bloxian",
      Subtitle = "link in pabtebin",
      Note = "join at my discord",
      FileName = "beat up bloxian", -- It is recommended to use something unique as other scripts using Rayfield may overwrite your key file
      SaveKey = false, -- The user's key will be saved, but if you change the key, they will be unable to use your script
      GrabKeyFromSite = true, -- If this is true, set Key below to the RAW site you would like Rayfield to get the key from
      Key = {"https://pastebin.com/fDw3tWaA"} -- List of keys that will be accepted by the system, can be RAW file links (pastebin, github etc) or simple strings ("hello","key22")
   }
})

local Tab = Window:CreateTab("home", in) -- Title, Image
local Section = mainTab:CreateSection("main)

Rayfield:Notify({
   Title = "you ececuted the script",
   Content = "very good gui",
   Duration = 5,
   Image = 4483362458,
   Actions = { -- Notification Buttons
      Ignore = {
         Name = "Okay!",
         Callback = function()
         print("The user tapped Okay!")
      end
   },
},
})

local Button = mainTab:CreateButton({
   Name = "infinite jump",
   Callback = function()
   -- The function that takes place when the button is pressed
   end,
})
