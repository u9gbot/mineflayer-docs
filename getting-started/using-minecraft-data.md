# Using Minecraft-Data

Using [minecraft-data](https://github.com/PrismarineJS/node-minecraft-data) should be one of the first steps of anybody using mineflayer, luckily it has a very simple api that is quick to learn. The best way to teach in programming is by doing, so here are a few examples of reasons you would need minecraft-data.

### Finding the id of an item

From very early, minecraft items have had an id, that is changed every minecraft version, so it is best to get this id dynamically.

1. Find an instance of [`minecraft-data`](https://github.com/PrismarineJS/node-minecraft-data) to use. minecraft-data comes bundled inside of mineflayer under `bot.registry`, which allows for quick access.
2. You can simply use `bot.registry.itemsByName.name.id` with name being the name of an item.
3. Find the name of the item in minecraft-data [using this website](https://minecraft-data.prismarine.js.org/?v=1.18.2). Make sure to select your minecraft version at the top, then select items, then search for the item you want, and write down the name from the name tab for later.
4. Use the name from step 3 with the object from step 2. For example, If I was looking for an iron sword, I would use `bot.registry.itemsByName.iron_sword.id`
