import discord
from discord.ext import commands

intents = discord.Intents.default()
intents.message_content = True

bot = commands.Bot(command_prefix='$', intents=intents)

@bot.event
async def on_ready():
    print(f'Estamos logados como {bot.user}')

@bot.command()
async def hello(ctx):
    await ctx.send(f'Olá! eu sou um bot {bot.user}!')

@bot.command()
async def heh(ctx, count_heh = 5):
    await ctx.send("he" * count_heh)
    
bot.run("MTQ3NjM1NTUwODQ5NDY2Nzk5OQ.G_O3ex.4CgYbN-ADLy1KSb4IciKkDQG11aAKiZXVXhb3Q")
