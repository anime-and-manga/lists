# Anime and Manga ID Mappings

This repository hosts JSON files containing ID mappings between AniList and MyAnimeList for both anime and manga. The purpose of these mappings is to facilitate easy cross-referencing between the two platforms.

## Files

- **anime.json**: Contains ID mappings for anime.
- **anime-with-titles.json**: Contains ID mappings and titles for anime.
- **manga.json**: Contains ID mappings for manga.
- **manga-with-titles.json**: Contains ID mappings and titles for manga.

## File Structure

JSON file follows this structure:

### anime.json / manga.json

```json
[
    {
        "idAL": 116589,
        "idMal": 41457,
    },
    {
        "idAL": 131586,
        "idMal": 48569,
    }
    ...
]
```

### anime-with-titles.json / manga-with-titles.json

```json
[
    {
        "idAL": 116589,
        "idMal": 41457,
        "title": {
            "romaji": "86: Eighty Six",
            "english": "86 EIGHTY-SIX",
            "native": "86－エイティシックス－"
        }
    },
    {
        "idAL": 131586,
        "idMal": 48569,
        "title": {
            "romaji": "86: Eighty Six Part 2",
            "english": "86 EIGHTY-SIX Part 2",
            "native": "86－エイティシックス－ 第2クール"
        }
    }
    ...
]
```

* `idAL`: The ID of the anime or manga on AniList.
* `idMal`: The corresponding ID of the anime or manga on MyAnimeList.
* `titles`: Contains the anime or manga title in the `romaji`, `english`, or `native` language.

## Usage

The IDs can be used as follows:

* `https://anilist.co/anime/<idAL>`
* `https://anilist.co/manga/<idAL>`
* `https://myanimelist.net/anime/<idMal>`
* `https://myanimelist.net/manga/<idMal>`

Replace `<idAL>` and `<idMal>` with the respective IDs from the JSON files.
