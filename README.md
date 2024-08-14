# Anime and Manga ID Mappings

This repository hosts JSON files containing ID mappings between AniList and MyAnimeList for both anime and manga. The purpose of these mappings is to facilitate easy cross-referencing between the two platforms.

## Files

- **anime.json**: Contains ID mappings for anime.
- **anime-full.json**: Contains ID mappings, titles and type for anime.
- **anime-airing.json**: Contains ID mappings, titles, and episode information for currently airing anime.
- **manga.json**: Contains ID mappings for manga.
- **manga-full.json**: Contains ID mappings, titles and type for manga.

## File Structure

JSON file follows this structure:

### anime.json / manga.json

```json
[
    {
        "idAL": 116589,
        "idAniDB":15441,
        "idMal": 41457,
    },
    {
        "idAL": 20954,
        "idAniDB": 10937,
        "idMal": 28851,
    }
    ...
]
```

### anime-full.json / manga-full.json

```json
[
    {
        "idAL": 116589,
        "idAniDB":15441,
        "idMal": 41457,
        "titles": {
            "romaji": "86: Eighty Six",
            "english": "86 EIGHTY-SIX",
            "native": "86－エイティシックス－"
        },
        "type": "TV"
    },
    {
        "idAL": 20954,
        "idAniDB": 10937,
        "idMal": 28851,
        "titles": {
            "romaji": "Koe no Katachi",
            "english": "A Silent Voice",
            "native": "聲の形"
        },
        "type": "MOVIE"
    }
    ...
]
```

### anime-airing.json

```json
[
    {
        "idAL": 145728,
        "idAniDB":17221,
        "idMal": 51122,
        "titles": {
            "romaji": "Ookami to Koushinryou: MERCHANT MEETS THE WISE WOLF",
            "english": "Spice and Wolf: MERCHANT MEETS THE WISE WOLF",
            "native": "狼と香辛料 MERCHANT MEETS THE WISE WOLF"
        },
        "type": "TV",
        "cover": "URL",
        "nsfw": false,
        "nextEpisode": {
            "episodeNumber": 2,
            "date": 1630000000
        }
    },
    ...
]
```

* `idAL`: The ID of the anime or manga on AniList.
* `idAniDB`: The ID of the anime or manga on AniDB.
* `idMal`: The corresponding ID of the anime or manga on MyAnimeList.
* `titles`: Contains the anime or manga title in the `romaji`, `english`, or `native` language.
* `type`: The media type/format.
* `cover`: URL to the cover image of the title.
* `nsfw`: Wheter the media is marked as adult or not.
* `nextEpisode`: Contains information about the next airing episode

## Usage

The IDs can be used as follows:

* `https://anilist.co/anime/<idAL>`
* `https://anilist.co/manga/<idAL>`
* `https://myanimelist.net/anime/<idMal>`
* `https://myanimelist.net/manga/<idMal>`
* `https://anidb.net/anime/<idAniDB>`

Replace `<idAL>` and `<idMal>` with the respective IDs from the JSON files.
