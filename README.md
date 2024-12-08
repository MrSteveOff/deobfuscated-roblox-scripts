# Deobfuscated Robloc Scripts 

Basically decompiles of many roblox script (for hacking ofc)

# How do i do it?

There are different ways to do it, but most of them use DL obfuscator or something, and i use this script for decomping that (the code is specifically for obfuscated codes like this: \32\32\108\111\99\97\108\32\112\108\97\121\101\114\32\61\32\103\97\109\):

local obfuscated = [[ -- put the obfuscated code here ]]

local decoded = obfuscated:gsub("\\(%d+)", function(n)
	return string.char(tonumber(n))
end)

print(decoded)
