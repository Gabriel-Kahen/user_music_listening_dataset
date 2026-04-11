GitHub mirror for the Kaggle dataset [`gabrielkahen/music-listening-data-500k-users`](https://www.kaggle.com/datasets/gabrielkahen/music-listening-data-500k-users) and its companion notebooks.

# Scope: ~500,000 Users

## Data Downloads

The dataset files are published as GitHub release assets instead of being committed into the repository.

CSV assets:

- `csv-users.csv`
- `csv-user_top_artists.csv`
- `csv-user_top_tracks.csv`
- `csv-user_top_albums.csv`

CSV schema:

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

DuckDB assets:

- `duckdb-bundle.zip`
- `duckdb-bundle.z01`

For the DuckDB download, place both files in the same folder and unzip `duckdb-bundle.zip`.

## Kaggle Sources

- Dataset: <https://www.kaggle.com/datasets/gabrielkahen/music-listening-data-500k-users>
- Notebook: <https://www.kaggle.com/code/gabrielkahen/artist-network>
- Notebook: <https://www.kaggle.com/code/gabrielkahen/top-artists>
