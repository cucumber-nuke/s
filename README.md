local MacLib = loadstring(game:HttpGet("https://github.com/biggaboy212/Maclib/releases/latest/download/maclib.txt"))()

local Window = MacLib:Window({
    Title = "CUCUMBER Hub 0.1",
    Subtitle = ".gg/UbTUdnq5Hw",
    Size = UDim2.fromOffset(868, 650),
    DragStyle = 1,
    DisabledWindowControls = {},
    ShowUserInfo = true,
    Keybind = Enum.KeyCode.RightShift,  -- Space key
    AcrylicBlur = true,
})

local globalSettings = {
	UIBlurToggle = Window:GlobalSetting({
		Name = "UI Blur",
		Default = Window:GetAcrylicBlurState(),
		Callback = function(bool)
			Window:SetAcrylicBlurState(bool)
			Window:Notify({
				Title = Window.Settings.Title,
				Description = (bool and "Enabled" or "Disabled") .. " UI Blur",
				Lifetime = 5
			})
		end,
	}),
	NotificationToggler = Window:GlobalSetting({
		Name = "Notifications",
		Default = Window:GetNotificationsState(),
		Callback = function(bool)
			Window:SetNotificationsState(bool)
			Window:Notify({
				Title = Window.Settings.Title,
				Description = (bool and "Enabled" or "Disabled") .. " Notifications",
				Lifetime = 5
			})
		end,
	}),
	ShowUserInfo = Window:GlobalSetting({
		Name = "Show User Info",
		Default = Window:GetUserInfoState(),
		Callback = function(bool)
			Window:SetUserInfoState(bool)
			Window:Notify({
				Title = Window.Settings.Title,
				Description = (bool and "Showing" or "Redacted") .. " User Info",
				Lifetime = 5
			})
		end,
	})
}

local tabGroups = {
    TabGroup1 = Window:TabGroup()
}

local tabs = {
    Main = tabGroups.TabGroup1:Tab({ Name = "📂ㅣMain", Image = "nil" }),
    Bedwars = tabGroups.TabGroup1:Tab({ Name = "🛏️ㅣBedwars", Image = "nil" }),
    Doors = tabGroups.TabGroup1:Tab({ Name = "🚪ㅣDoors", Image = "nil" }),
    Arsenal = tabGroups.TabGroup1:Tab({ Name = "🔫ㅣArsenal", Image = "nil" }),
    Rivals = tabGroups.TabGroup1:Tab({ Name = "🔫ㅣRivals", Image = "nil" }),
    Legendofspeed = tabGroups.TabGroup1:Tab({ Name = "🏃ㅣLegend Of Speed", Image = "nil" }),
    Navalwarfare = tabGroups.TabGroup1:Tab({ Name = "⚓ㅣNaval Warfare", Image = "nil" }),
    Prisonlife = tabGroups.TabGroup1:Tab({ Name = "👮ㅣPrison Life", Image = "nil" }),
    Slapbattles = tabGroups.TabGroup1:Tab({ Name = "👋ㅣSlap battles", Image = "nil" }),
    Bloxfruits = tabGroups.TabGroup1:Tab({ Name = "🍈ㅣBlox Fruits", Image = "nil" }),
    Murdermystery2 = tabGroups.TabGroup1:Tab({ Name = "🔪ㅣMurder Mystery 2", Image = "nil" }),
    Bladeball = tabGroups.TabGroup1:Tab({ Name = "🏓ㅣBlade Ball", Image = "nil" }),
    Combatwarriors = tabGroups.TabGroup1:Tab({ Name = "⚔️ㅣCombat Warriors", Image = "nil" }),
    Zombieattack = tabGroups.TabGroup1:Tab({ Name = "🧟ㅣZombie Attack", Image = "nil" }),
    Memesea = tabGroups.TabGroup1:Tab({ Name = "🤣ㅣMeme Sea", Image = "nil" }),
    Koreaminecraft = tabGroups.TabGroup1:Tab({ Name = "🇰🇷ㅣKorea Minecraft", Image = "nil" }),
    Funkyfriday = tabGroups.TabGroup1:Tab({ Name = "🎤ㅣFunky Friday", Image = "nil" }),
    Tsb = tabGroups.TabGroup1:Tab({ Name = "💪ㅣTSB", Image = "nil" }),
    Dahood = tabGroups.TabGroup1:Tab({ Name = "🖕🏿ㅣDa Hood", Image = "nil" }),
    Mvsd = tabGroups.TabGroup1:Tab({ Name = "🛡️ㅣMVSD", Image = "nil" }),
    Kinglegacy = tabGroups.TabGroup1:Tab({ Name = "👑ㅣKing Legacy", Image = "nil" }),
    Adustytrip = tabGroups.TabGroup1:Tab({ Name = "🛢️ㅣA Dusty Trip", Image = "nil" }),
    Credit = tabGroups.TabGroup1:Tab({ Name = "📼ㅣCredit", Image = "nil" }),
    Changelog = tabGroups.TabGroup1:Tab({ Name = "🎲ㅣChange Log", Image = "nil" }),
}

local mainSection = tabs.Main:Section({ Side = "Left" })

mainSection:Button({
    Name = "infinity jump",
    Callback = function()
	loadstring(game:HttpGet("https://pastebin.com/raw/WweihvrM"))()
        Window:Notify({
            Title = "Main",
            Description = "infinity jump executed!",
        })
    end,
})

mainSection:Button({
    Name = "Fly",
    Callback = function()
	loadstring(game:HttpGet(('https://pastebin.com/raw/dACYznRK'),true))()
        Window:Notify({
            Title = "Main",
            Description = "fly executed!",
        })
    end,
})

mainSection:Button({
    Name = "Esp",
    Callback = function()
	loadstring(game:HttpGet(('https://pastebin.com/raw/7K1Jhmck'),true))()
        Window:Notify({
            Title = "Main",
            Description = "esp executed!",
        })
    end,
})

mainSection:Button({
    Name = "infinity yield",
    Callback = function()
	loadstring(game:HttpGet(('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'),true))()
        Window:Notify({
            Title = "Main",
            Description = "IY executed!",
        })
    end,
})

mainSection:Button({
    Name = "dark dex",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/Babyhamsta/RBLX_Scripts/main/Universal/BypassedDarkDexV3.lua", true))()
        Window:Notify({
            Title = "Main",
            Description = "dark dex executed!",
        })
    end,
})

mainSection:Button({
    Name = "see level",
    Callback = function()
	printidentity()
        Window:Notify({
            Title = "Main",
            Description = "press F9 to see level!",
        })
    end,
})

mainSection:Button({
    Name = "see unc",
    Callback = function()
	loadstring(game:HttpGet(('https://raw.githubusercontent.com/cucumber-nuke/unc/refs/heads/main/.gitignore'),true))()
        Window:Notify({
            Title = "Main",
            Description = "sUNC test, press F9 to see level!",
        })
    end,
})

mainSection:Button({
    Name = "FE animation",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/Gazer-Ha/Animated/main/G"))()
        Window:Notify({
            Title = "Main",
            Description = "FE animation executed!",
        })
    end,
})

mainSection:Button({
    Name = "copy game(need wait)",
    Callback = function()
	saveinstance()
        Window:Notify({
            Title = "Main",
            Description = "copy game executed!",
        })
    end,
})

mainSection:Button({
    Name = "FE sus script",
    Callback = function()
	game.Players.LocalPlayer:Kick("You're a pervert.")
        Window:Notify({
            Title = "Main",
            Description = "fuck you, pervert. you are an idiot and niga bitch.",
        })
    end,
})

mainSection:Button({
    Name = "Destroy server(some games don't work)",
    Callback = function()
	loadstring(game:HttpGet(('https://pastebin.com/raw/B6WLJDw0'),true))()
        Window:Notify({
            Title = "Main",
            Description = "Destroy server executed!(some games don't work",
        })
    end,
})

mainSection:Button({
    Name = "invisible(toggle - G)",
    Callback = function()
	loadstring(game:HttpGet(('https://pastebin.com/raw/Sutx6evH'),true))()
        Window:Notify({
            Title = "Main",
            Description = "invisible executed!",
        })
    end,
})

mainSection:Button({
    Name = "nameless admin",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/FilteringEnabled/NamelessAdmin/main/Source"))();
        Window:Notify({
            Title = "Main",
            Description = "nameless admin script executed!",
        })
    end,
})

mainSection:Button({
    Name = "aim bot",
    Callback = function()
	loadstring(game:HttpGet("https://pastebin.com/raw/utHyEcbk"))()
        Window:Notify({
            Title = "Main",
            Description = "aim bot executed!",
        })
    end,
})

local bedwarsSection = tabs.Bedwars:Section({ Side = "Left" })

bedwarsSection:Button({
    Name = "Alsploit",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/AlSploit/AlSploit/main/AlSploit/Bedwars/Loader.lua"))() 
        Window:Notify({
            Title = "Main",
            Description = "Alsploit executed!",
        })
    end,
})

bedwarsSection:Button({
    Name = "Aurora",
    Callback = function()
	loadstring(game:HttpGet('https://raw.githubusercontent.com/cocotv666/Aurora/refs/heads/main/Aurora_Loader'))()
        Window:Notify({
            Title = "Main",
            Description = "Aurora executed!",
        })
    end,
})

bedwarsSection:Button({
    Name = "CoCoSploit",
    Callback = function()
	loadstring(game:HttpGet('https://raw.githubusercontent.com/cocotv666/CocoSploit/main/CocoSploit_Loader'))()
        Window:Notify({
            Title = "Main",
            Description = "CoCoSploit executed!",
        })
    end,
})

bedwarsSection:Button({
    Name = "Vape V4",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/7GrandDadPGN/VapeV4ForRoblox/main/NewMainScript.lua", true))()
        Window:Notify({
            Title = "Main",
            Description = "Vape V4 executed!",
        })
    end,
})

bedwarsSection:Button({
    Name = "Snyware",
    Callback = function()
	loadstring(game:HttpGet('https://raw.githubusercontent.com/AFGCLIENT/Snyware/main/Loader'))()
        Window:Notify({
            Title = "Main",
            Description = "Snyware executed!",
        })
    end,
})

bedwarsSection:Button({
    Name = "Voidware",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/VapeVoidware/vapevoidware/main/NewMainScript.lua", true))()
        Window:Notify({
            Title = "Main",
            Description = "Voidware executed!",
        })
    end,
})

bedwarsSection:Button({
    Name = "CAT Vape Installer",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/qwertyui-is-back/CatV5/refs/heads/main/Libraries/Installer.lua"))()
        Window:Notify({
            Title = "Main",
            Description = "CV executed!",
        })
    end,
})

bedwarsSection:Button({
    Name = "cat vape(no log in)",
    Callback = function()
	loadfile("catvape/loader.lua")()
        Window:Notify({
            Title = "Main",
            Description = "CV executed!",
        })
    end,
})

bedwarsSection:Button({
    Name = "cat vape discord",
    Callback = function()
	setclipboard("https://discord.gg/88EEN4M8Pq")
        Window:Notify({
            Title = "Main",
            Description = "CV executed!",
        })
    end,
})

local doorsSection = tabs.Doors:Section({ Side = "Left" })

doorsSection:Button({
    Name = "doors hub",
    Callback = function()
	loadstring(game:HttpGet(('https://pastebin.com/raw/9QPGnLx6'),true))()
        Window:Notify({
            Title = "Main",
            Description = "doors hub executed!",
        })
    end,
})

doorsSection:Button({
    Name = "mspaint",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/notpoiu/mspaint/main/main.lua"))()
        Window:Notify({
            Title = "Main",
            Description = "mspaint executed!",
        })
    end,
})

doorsSection:Button({
    Name = "blacking hub",
    Callback = function()
	loadstring(game:HttpGetAsync("https://pastebin.com/raw/R8QMbhzv"))()
        Window:Notify({
            Title = "Main",
            Description = "blacking hub executed!",
        })
    end,
})

doorsSection:Button({
    Name = "FFJ",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/FFJ1/Roblox-Exploits/main/scripts/Loader.lua"))()
        Window:Notify({
            Title = "Main",
            Description = "FFJ executed!",
        })
    end,
})

doorsSection:Button({
    Name = "Zygarde",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/louismich4el/Zygarde/main/Protected%20zygarde.lua"))()
        Window:Notify({
            Title = "Main",
            Description = "Zygarde executed!",
        })
    end,
})

local arsenalSection = tabs.Arsenal:Section({ Side = "Left" })

arsenalSection:Button({
    Name = "Quotas HUB",
    Callback = function()
	loadstring(game:HttpGet("https://pastebin.com/raw/8ysy7ENG",true))()
        Window:Notify({
            Title = "Main",
            Description = "Quotas HUB executed!",
        })
    end,
})

arsenalSection:Button({
    Name = "Solaris",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/toasty-dev/pissblox/main/solaris_bootstrapper.lua",true))()
        Window:Notify({
            Title = "Main",
            Description = "Solara... oh Solaris executed!",
        })
    end,
})

arsenalSection:Button({
    Name = "Thunder Client V2",
    Callback = function()
	loadstring(game:HttpGet(('https://pastebin.com/raw/eFEffwsy'),true))()
        Window:Notify({
            Title = "Main",
            Description = "Thender Client V2 executed!",
        })
    end,
})

arsenalSection:Button({
    Name = "HOHO HUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/acsu123/HOHO_H/main/Loading_UI"))()
        Window:Notify({
            Title = "Main",
            Description = "HOHO HUB executed!",
        })
    end,
})

arsenalSection:Button({
    Name = "QP HUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/QPScript/Script/main/Arsenal.txt"))()
        Window:Notify({
            Title = "Main",
            Description = "QP GAY Hub executed!",
        })
    end,
})

arsenalSection:Button({
    Name = "Leg HUB",
    Callback = function()
	loadstring(game:HttpGet("https://pastebin.com/raw/G6Ubkkuv"))()
        Window:Notify({
            Title = "Main",
            Description = "leg hub executed!",
        })
    end,
})

arsenalSection:Button({
    Name = "Virtual Hub",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/DomainXV3/DomainX/main/virtual.cc",true))()
        Window:Notify({
            Title = "Main",
            Description = "Virtual Hub executed!",
        })
    end,
})

arsenalSection:Button({
    Name = "Tanqr HUB",
    Callback = function()
	loadstring(game:HttpGet("https://pastebin.com/raw/mXQLj82U"))()
        Window:Notify({
            Title = "Main",
            Description = "Tanqr HUB executed",
        })
    end,
})

local rivalSection = tabs.Rivals:Section({ Side = "Left" })

rivalsSection:Button({
    Name = "Vape V4",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/7GrandDadPGN/VapeV4ForRoblox/main/NewMainScript.lua", true))()
        Window:Notify({
            Title = "Main",
            Description = "Vape V4 executed!",
        })
    end,
})

rivalsSection:Button({
    Name = "Tbao HUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/tbao143/thaibao/main/TbaoHubRivals"))()
        Window:Notify({
            Title = "Main",
            Description = "Tbao hub executed!",
        })
    end,
})

rivalsSection:Button({
    Name = "Thunder Client",
    Callback = function()
	loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/25bef65fd4756876a25c68d1297b80a6.lua"))()
        Window:Notify({
            Title = "Main",
            Description = "Thunder Client executed!",
        })
    end,
})

rivalsSection:Button({
    Name = "Phantom HUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/5oxin/Phantom/main/main"))()
        Window:Notify({
            Title = "Main",
            Description = "phantom hub executed!",
        })
    end,
})

rivalsSection:Button({
    Name = "LB HUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/LOLking123456/RIVALS/main/Roblox"))()
        Window:Notify({
            Title = "Main",
            Description = "LB hub executed!",
        })
    end,
})

local legendofspeedSection = tabs.Legendofspeed:Section({ Side = "Left" })

legendofspeedSection:Button({
    Name = "EZ HUB",
    Callback = function()
	loadstring(game:HttpGet(('https://raw.githubusercontent.com/debug42O/Ez-Industries-Launcher-Data/master/Launcher.lua'),true))()
        Window:Notify({
            Title = "Main",
            Description = "fuck you lol "ez" gg",
        })
    end,
})

legendofspeedSection:Button({
    Name = "Tbao HUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/tbao143/thaibao/main/TbaoHublegendsofspeed"))()
        Window:Notify({
            Title = "Main",
            Description = "Tbao executed!",
        })
    end,
})

legendofspeedSection:Button({
    Name = "itzperson.ru hub",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/od1ri/Legends-Of-Speed/main/loadstring.lua"))()
        Window:Notify({
            Title = "Main",
            Description = "it's person.ru executed!",
        })
    end,
})

legendofspeedSection:Button({
    Name = "LOS HUB",
    Callback = function()
	loadstring(game:HttpGet('https://raw.githubusercontent.com/StupidProAArsenal/main/main/Legenos%20of%20speedos'))()
        Window:Notify({
            Title = "Main",
            Description = "LOS executed!",
        })
    end,
})

legendofspeedSection:Button({
    Name = "Relz HUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/farghii/relzhub/main/execute.hack", true))()
        Window:Notify({
            Title = "Main",
            Description = "Relz executed!",
        })
    end,
})

local navalwarfareSection = tabs.Navalwarfare:Section({ Side = "Left" })

navalwarfareSection:Button({
    Name = "NW HUB",
    Callback = function()
	loadstring(game:HttpGet('https://raw.githubusercontent.com/hussain1323232234/My-Scripts/main/Naval%20Warfare'))()
        Window:Notify({
            Title = "Main",
            Description = "NW executed!",
        })
    end,
})

local prisonlifeSection = tabs.Prisonlife:Section({ Side = "Left" })

prisonlifeSection:Button({
    Name = "Tbao HUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/tbao143/thaibao/main/TbaohubPrisonLife"))()
        Window:Notify({
            Title = "Main",
            Description = "Tbao executed!",
        })
    end,
})

prisonlifeSection:Button({
    Name = "Tiger Admin",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/dalloc2/Roblox/main/TigerAdmin.lua"))()
        Window:Notify({
            Title = "Main",
            Description = "Tiger admin executed!",
        })
    end,
})

prisonlifeSection:Button({
    Name = "prisonware",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/Denverrz/scripts/master/PRISONWARE_v1.3.txt"))();
        Window:Notify({
            Title = "Main",
            Description = "prisonware executed!",
        })
    end,
})

prisonlifeSection:Button({
    Name = "FE GUI",
    Callback = function()
	loadstring("\108\111\97\100\115\116\114\105\110\103\40\103\97\109\101\58\72\116\116\112\71\101\116\40\34\104\116\116\112\115\58\47\47\114\97\119\46\103\105\116\104\117\98\117\115\101\114\99\111\110\116\101\110\116\46\99\111\109\47\103\48\48\108\88\112\108\111\105\116\101\114\47\103\48\48\108\88\112\108\111\105\116\101\114\47\109\97\105\110\47\70\101\37\50\48\98\121\112\97\115\115\34\44\32\116\114\117\101\41\41\40\41\10")()
        Window:Notify({
            Title = "Main",
            Description = "FE GUI executed!",
        })
    end,
})

prisonlifeSection:Button({
    Name = "Lightux HUB",
    Callback = function()
	loadstring(game:HttpGet(('https://raw.githubusercontent.com/cool83birdcarfly02six/Lightux/main/README.md'),true))()
        Window:Notify({
            Title = "Main",
            Description = "Lightux Hubexecuted!",
        })
    end,
})

prisonlifeSection:Button({
    Name = "Prizzlife",
    Callback = function()
	loadstring(game:HttpGet('https://raw.githubusercontent.com/elliexmln/PrizzLife/main/pladmin.lua'))()
        Window:Notify({
            Title = "Main",
            Description = "prizzlife executed!",
        })
    end,
})

local slapbattlesSection = tabs.Slapbattles:Section({ Side = "Left" })

slapbattlesSection:Button({
    Name = "Article Hub",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/Playgiang/Slap_Battles/main/Slap_Battles.lua"))()
        Window:Notify({
            Title = "Main",
            Description = "Article(giang hub) executed!",
        })
    end,
})

slapbattlesSection:Button({
    Name = "Free titan",
    Callback = function()
	loadstring(game:HttpGet(('https://pastebin.com/raw/6fY2UcjM'),true))()
        Window:Notify({
            Title = "Main",
            Description = "see back pack!",
        })
    end,
})

local bloxfruitsSection = tabs.Bloxfruits:Section({ Side = "Left" })

bloxfruitsSection:Button({
    Name = "REDzHUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/REDzHUB/BloxFruits/main/redz9999"))()
        Window:Notify({
            Title = "Main",
            Description = "REDzHUB executed!",
        })
    end,
})

bloxfruitsSection:Button({
    Name = "HoHo HUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/acsu123/HOHO_H/main/Loading_UI"))()
        Window:Notify({
            Title = "Main",
            Description = "HoHo HUB executed!",
        })
    end,
})

bloxfruitsSection:Button({
    Name = "MinGaming HUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/SkibidiSupremacy/Loader.xyz/main/Pronto.yxz%20ST%20%3A%20G"))()
        Window:Notify({
            Title = "Main",
            Description = "KEY : xk06nst6bgj8a",
        })
    end,
})

bloxfruitsSection:Button({
    Name = "LunarXHUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/NguyenLam2504/LunarXHubNextGeneration/main/GameShit.lua"))()
        Window:Notify({
            Title = "Main",
            Description = "LunarXHUB executed!",
        })
    end,
})

bloxfruitsSection:Button({
    Name = "Sea Gate HUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/SkibidiSupremacy/Loader.xyz/main/NextGen"))()
        Window:Notify({
            Title = "Main",
            Description = "Sea Gate HUB executed!",
        })
    end,
})

bloxfruitsSection:Button({
    Name = "Speed X HUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/AhmadV99/Script-Games/main/Blox%20Fruit.lua"))()
        Window:Notify({
            Title = "Main",
            Description = "Speed X HUB executed!",
        })
    end,
})

bloxfruitsSection:Button({
    Name = "MinGaming HUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/Basicallyybeta/mingane/main/MinGamingNew.lua"))()
        Window:Notify({
            Title = "Main",
            Description = "MinGaming HUB executed!",
        })
    end,
})

bloxfruitsSection:Button({
    Name = "Vector HUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/AAwful/VectorHub/main/Loader.lua"))()
        Window:Notify({
            Title = "Main",
            Description = "Vector HUB",
        })
    end,
})

bloxfruitsSection:Button({
    Name = "Relz HUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/farghii/relzhub/main/execute.hack", true))()
        Window:Notify({
            Title = "Main",
            Description = "Relz HUB executed!",
        })
    end,
})

local murdermystery2Section = tabs.Murdermystery2:Section({ Side = "Left" })

murdermystery2Section:Button({
    Name = "Byte HUB",
    Callback = function()
	loadstring(game:HttpGet("https://pastebin.com/raw/mMqS6s5F"))()
        Window:Notify({
            Title = "Main",
            Description = "Byte HUB executed!",
        })
    end,
})

murdermystery2Section:Button({
    Name = "Haxhell HUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/haxhell/roblox-scripts/main/murder-mystery-2.lua", true))()
        Window:Notify({
            Title = "Main",
            Description = "Haxhell HUB executed!",
        })
    end,
})

murdermystery2Section:Button({
    Name = "YARHM HUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/Joystickplays/psychic-octo-invention/main/yarhm.lua", false))()
        Window:Notify({
            Title = "Main",
            Description = "YARHM HUB executed!",
        })
    end,
})

murdermystery2Section:Button({
    Name = "Ghost HUB",
    Callback = function()
	loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/GhostHub'))()
        Window:Notify({
            Title = "Main",
            Description = "Ghost HUB executed!",
        })
    end,
})

murdermystery2Section:Button({
    Name = "Vynixu HUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/Neon-Fox/roblox-scripts/main/VynixuMM2"))()
        Window:Notify({
            Title = "Main",
            Description = "Vynixu HUB executed!",
        })
    end,
})

murdermystery2Section:Button({
    Name = "Zygarde HUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/louismich4el/Zygarde/main/Protected%20zygarde.lua"))()
        Window:Notify({
            Title = "Main",
            Description = "Zygarde HUB executed",
        })
    end,
})

local bladeballSection = tabs.Blade ball:Section({ Side = "Left" })

bladeballSection:Button({
    Name = "Pitbull HUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/SoyAdriYT/PitbullHubX/main/Loader.lua", true))()
        Window:Notify({
            Title = "Main",
            Description = "Pitbull HUB executed!",
        })
    end,
})

bladeballSection:Button({
    Name = "Nexam HUB",
    Callback = function()
	loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/6af56c1753ac6679dee3acbd1fd952e5.lua"))()
        Window:Notify({
            Title = "Main",
            Description = "Nexam HUB executed!",
        })
    end,
})

bladeballSection:Button({
    Name = "Astral HUB",
    Callback = function()
	loadstring(game:HttpGet('https://raw.githubusercontent.com/Augustzyzx/A-s-t-r-a-l/main/Loader_BladeBall.lua'))()
        Window:Notify({
            Title = "Main",
            Description = "Astral HUB executed!",
        })
    end,
})

bladeballSection:Button({
    Name = "Visual V3.5",
    Callback = function()
	loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/a5945467f3b9388503ca653c0ea49cba.lua"))()
        Window:Notify({
            Title = "Main",
            Description = "Visual V3.5 executed!",
        })
    end,
})

bladeballSection:Button({
    Name = "Pitbull HUB",
    Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/SoyAdriYT/PitbullHub--/main/Destroyer", true))()
        Window:Notify({
            Title = "Main",
            Description = "Pitbull HUB executed!",
        })
    end,
})

local combatwarriorsSection = tabs.Combatwarriors:Section({ Side = "Left" })

combatwarriorsSection:Button({
    Name = "Head Hitbox",
    Callback = function()
	loadstring(game:HttpGet("https://pastebin.com/raw/UauTz6D4"))()
        Window:Notify({
            Title = "Main",
            Description = "Head Hitbox",
        })
    end,
})

combatwarriorsSection:Button({
    Name = "Stratos HUB",
    Callback = function()
	loadstring(game:HttpGet("https://pastefy.app/50B4Z9UK/raw"))()
        Window:Notify({
            Title = "Main",
            Description = "Stratos HUB",
        })
    end,
})

combatwarriorsSection:Button({
    Name = "MaxHUB",
    Callback = function()
	loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/1d4db6a1b04aaeccf046f7c63fbad31a.lua"))()
        Window:Notify({
            Title = "Main",
            Description = "MaxHUB",
        })
    end,
})

local zombieattackSection = tabs.Zombieattack:Section({ Side = "Left" })

zombieattackSection:Button({
    Name = "Ski HUB",
    Callback = function()
	loadstring(game:HttpGet(("https://pastebin.com/raw/mT10xnt7"), true))()
        Window:Notify({
            Title = "Main",
            Description = "Ski HUB executed!",
        })
    end,
})

zombieattackSection:Button({
    Name = "Voidz HUB",
    Callback = function()
	loadstring(game:HttpGet(('https://raw.githubusercontent.com/RTrade/Voidz/main/Games.lua'),true))()
        Window:Notify({
            Title = "Main",
            Description = "Voidz HUB",
        })
    end,
})

local memeseaSection = tabs.Memesea:Section({ Side = "Left" })

local koreaminecraftSection = tabs.Koreaminecraft:Section({ Side = "Left" })

local funkyfridaySection = tabs.Funkyfriday:Section({ Side = "Left" })

local tsbSection = tabs.Tsb:Section({ Side = "Left" })

local dahoodSection = tabs.Dahood:Section({ Side = "Left" })

local mvsdSection = tabs.Mvsd:Section({ Side = "Left" })

local kinglegacySection = tabs.Kinglegacy:Section({ Side = "Left" })

local adustytripSection = tabs.adustytrip:Section({ Side = "Left" })

Window.onUnloaded(function()
    print("UI has been unloaded!")
end)

tabs.Main:Select()
