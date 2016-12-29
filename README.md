TODO: better README;

A simple script to show spawn points statistics for Pokemon GO, mainly for nest evaluation.
This script reads an "pokealert_spawn_points.json" file, which can be generated by the PokeAlert scanner tool (Android), and presents its data in a more readable way. Its main use is to check if some tracked area in that app is a nest on Pokemon GO.

For now it requires some manual configuration of the files inside data folder:
> common_pokemon.json - Here goes the GLOBAL list of common pokemons, which will be ignored when considering nests, although statistics for them are still presented. For a location-based list of commons, specify it on the next file.
> locs.json - You will need to create it or edit the "locs-example.json" file and save it as "locs.json". At least one location (real or not) must be specified before running the script. Other locations can be added on-the-fly.
> pokealert_spawn_points.json - This is the file you will need to export from the PokeAlert scanner tool (Android). An example file is provided, although unnecessary.
> pokemon_list.json - Here goes a list of all pokemons until Generation VI, sorted by theirs IDs. No need to mess with it, unless Pokemon GO gets Generation VII.

After configuring those files, install the requirements.txt as follow:
pip install -r requirements.txt

Finally, run the script: nestParser.py
