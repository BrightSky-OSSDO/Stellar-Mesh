# Stellar Mesh
The Stellar Mesh is a network of servers throughout space, created with the intention of revolutionizing space exploration and establishing space communication, opening up possibilities for interplanetary video conferencing and text messaging between astronauts, or even interplanetary VPNs.

# Compatibility
The Stellar Mesh can be used with any programming language that can parse JSON. If your desired progamming language doesn't have a built-in JSON parser, you will need to write one yourself.

# Syntax
The Stellar Mesh follows a specific syntax for each JSON file. Every celestial body's JSON file should contain this information, in this specific order:

- `name`: The celestial body's name. String value.
- `type`: The type of celestial body (planet, moon, or star). Asteroids and the Asteroid Belt count as planets. String value.
- `surface_temperature`: The average surface temperature of the celestial body in degrees Celcius. Must be an integer value. If the average surface temperature is a decimal number, it must be rounded to an integer.
- `gravity`: The gravitational force of the celestial body in m/s² (meters per second squared). Must be a decimal value with 2 decimal places. If the gravitational force is an integer, ".00" must be appended to the end. For example, 5 would become 5.00. If the celestial body has no gravitational force, this value should be set to null.
- `day`: The amount of time it takes for the celestial body to complete a full rotation on its axis, measured in Earth hours. Must be an integer value. If the day length is a decimal number, it must be rounded to an integer. If the celestial body doesn't rotate, this value should be set to null.
- `year`: The amount of time it takes for the celestial body to make a full trip around its parent object, measured in Earth days. Must be an integer value. If the year length is a decimal number, it must be rounded to an integer. If the celestial body doesn't orbit anything, this value should be set to null.
- `rings`: Whether or not the celestial body has a ring system. Boolean value.
- `parent`: The name of the object around which the celestial body orbits. Must be a string value. If the celestial body doesn't orbit anything, this value should be set to null.
- `satellites`: The number of natural satellites that orbit the celestial body. Integer value. For a planet, this value would refer to moons. For a star, this value would refer to planets. For a moon, this value would likely be 0 because most moons don't have natural satellites. **Note**: `satellites` does not include man-made objects that orbit a celestial body.
- `atmosphere`: A literal that contains information about the celestial body's atmosphere, including:
    - `corrosive`: Whether or not the atmosphere is corrosive. Boolean value. If the celestial body has no atmosphere, this value should be set to null.
    - `breathable`: Whether or not the atmosphere is breathable by humans. Boolean value. If the celestial body has no atmosphere, this value should be set to null.
- `server`: A boolean value indicating the presence or absence of a Stellar Mesh server on the celestial body. This value should always be set to true.

Please note that this syntax is subject to change in the future. However, rest assured that any changes made will be outlined in this README.

# Using the Stellar Mesh in Your Own Software
To use the Stellar Mesh in your own software project, you have 2 choices:

- Making a HTTP request to the files directly from this repository, and parsing the JSON files
- Downloading the repository to your local file system, placing them in your project's folder, and parsing the JSON files

It's recommended to download the repository to your local file system, especially if you're developing a software that can be used offline. But if you don't care about offline use, you can feel free to just make a HTTP request to the repository instead.

And, as mentioned earlier, the programming language you're using in your software project must be able to parse JSON, and if it doesn't have a built-in JSON parser you will need to write a custom one yourself.

# License
The Stellar Mesh is released under the Unlicense.

# Quotes
To fit the theme, here are some of my favorite quotes about space exploration:

> That's one small step for man, one giant leap for mankind.

*- Neil Armstrong*

---

> Somewhere, something incredible is waiting to be known.

*- Carl Sagan*

---

> I know the sky is not the limit because there are footprints on the Moon -- and I made some of them!

*- Buzz Aldrin*

---

> I think we are at the dawn of a new era in commercial space exploration.

*- Elon Musk*

# Future Plans
Currently, the Stellar Mesh only covers the Sun (Sol), Venus, Earth, Mars, the Asteroid Belt, and the Moon (Luna). However, there are big plans for the future; plans as big as expanding the Stellar Mesh to include exoplanets in addition to members of our solar system!
