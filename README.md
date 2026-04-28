# Music Listening History Dataset: 500k Users, Top Artists, Tracks, Albums, and Playcounts

Large-scale music listening dataset with user-level top artists, tracks, and albums for approximately 500,000 users. The data includes playcounts, rankings, user countries, and MusicBrainz IDs where available, making it useful for recommender systems, collaborative filtering, music taste modeling, personalization research, user behavior analysis, and music analytics.

This repository is the GitHub mirror for the Kaggle dataset [`gabrielkahen/music-listening-data-500k-users`](https://www.kaggle.com/datasets/gabrielkahen/music-listening-data-500k-users) and its companion notebooks.

## Dataset at a Glance

| Field | Details |
| --- | --- |
| Users | Approximately 500,000 |
| Tables | Users, user top artists, user top tracks, user top albums |
| Formats | CSV files and DuckDB bundle |
| Core fields | `user_id`, `country`, `rank`, `artist_name`, `track_name`, `album_name`, `playcount`, `mbid` |
| External identifiers | MusicBrainz IDs where available |
| Primary Kaggle page | <https://www.kaggle.com/datasets/gabrielkahen/music-listening-data-500k-users> |

## Use Cases

This dataset is designed for projects that need Last.fm-style user listening histories, user-artist interactions, user-track interactions, playcount data, and music preference data at a larger scale than many small demo datasets.

Common use cases include:

- Music recommender systems
- Collaborative filtering
- User listening history analysis
- Music taste modeling
- Music personalization research
- Artist similarity and user similarity
- Top artist, top track, and top album analytics
- MusicBrainz-linked music data analysis
- Country-level music preference analysis
- Dataset practice for DuckDB, pandas, SQL, and data visualization

## Data Downloads

The dataset files are published as GitHub release assets instead of being committed into the repository.

CSV assets:

- `csv-users.csv`
- `csv-user_top_artists.csv`
- `csv-user_top_tracks.csv`
- `csv-user_top_albums.csv`

DuckDB assets:

- `duckdb-bundle.zip`
- `duckdb-bundle.z01`

For the DuckDB download, place both files in the same folder and unzip `duckdb-bundle.zip`.

## CSV Schema

`csv-users.csv`

- `user_id`: integer user identifier.
- `country`: self-reported country name.
- `total_scrobbles`: total number of listens recorded for the user.

`csv-user_top_artists.csv`

- `user_id`: integer user identifier.
- `rank`: position in the user's top-artist list.
- `artist_name`: artist name.
- `playcount`: number of listens for that artist by the user.
- `mbid`: MusicBrainz identifier for the artist when available.

`csv-user_top_tracks.csv`

- `user_id`: integer user identifier.
- `rank`: position in the user's top-track list.
- `track_name`: track title.
- `artist_name`: track artist name.
- `playcount`: number of listens for that track by the user.
- `mbid`: MusicBrainz identifier for the track when available.

`csv-user_top_albums.csv`

- `user_id`: integer user identifier.
- `rank`: position in the user's top-album list.
- `album_name`: album title.
- `artist_name`: album artist name.
- `playcount`: number of listens for that album by the user.
- `mbid`: MusicBrainz identifier for the album when available.

## Companion Notebooks

- [Artist network](https://www.kaggle.com/code/gabrielkahen/artist-network): builds an artist co-listening network from user top artists.
- [Top artists](https://www.kaggle.com/code/gabrielkahen/top-artists): explores global and country-level top artists.

## Related Search Terms

People looking for this dataset may also search for music recommendation dataset, music recommender systems dataset, collaborative filtering music dataset, Last.fm-style listening history dataset, user listening history data, music user behavior dataset, user-artist interaction data, music playcount dataset, MusicBrainz dataset, and music analytics dataset.
