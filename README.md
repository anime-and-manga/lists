# Anime and Manga ID Mappings

This repository hosts JSON files containing ID mappings between AniList and MyAnimeList for both anime and manga. The purpose of these mappings is to facilitate easy cross-referencing between the two platforms.

## Files

- **anime.json**: Contains ID mappings for anime.
- **manga.json**: Contains ID mappings for manga.

## File Structure

Each JSON file follows this structure:

```json
[
    {
        "idAL": 116589,
        "idMal": 41457
    },
    {
        "idAL": 131586,
        "idMal": 48569
    }
    ...
]
```

* `idAL`: The ID of the anime or manga on AniList.
* `idMal`: The corresponding ID of the anime or manga on MyAnimeList.

## Usage

The IDs can be used as follows:

* `https://anilist.co/anime/<idAL>`
* `https://anilist.co/manga/<idAL>`
* `https://myanimelist.net/anime/<idMal>`
* `https://myanimelist.net/manga/<idMal>`

Replace `<idAL>` and `<idMal>` with the respective IDs from the JSON files.
