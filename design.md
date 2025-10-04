# Examples

## Sequencing

Play a track:

> mplay track.mp3

Play tracks in sequence:

> mplay track-01.mp3 track-02.mp3

The "sequence" command is implicit if no other command is given.
So, the following is equivalent to the above:

> mplay sequence track-01.mp3 track-02.mp3

Play all tracks in a directory, in order (by name)

> mplay ~/files/audio/music/artist/album

Play all tracks in the current directory:

> mplay .

Play albums in sequence:

> mplay /path/to/album-1 /path/to/album-2

## Shuffling

Shuffle a set of tracks:

> mplay shuffle track-01.mp3 track-02.mp3 track-03.mp3

Shuffle an album:

> mplay shuffle /path/to/album

Shuffle a set of albums:

> mplay shuffle /path/to/album-1 /path/to/album-2

Play an album, then shuffle a playlist:

> mplay /path/to/album, shuffle /path/to/playlist

Loop:
- Pick a random song from one playlist
- Pick a random song from another playlist

> mplay interleave shuffle /path/to/playlist-1, shuffle /path/to/playlist-2

## Interleaving

Loop:
- Play the next song from one album
- Play the next song from another album

> mplay interleave /path/to/album-1 /path/to/album-2

## Looping

Loop through a sequence of tracks:

> mplay loop track-01.mp3 track-02.mp3 track-03.mp3

Loop shuffling a playlist (infinite shuffle):

> mplay loop shuffle /path/to/playlist

Loop:
- Shuffle a set of playlists
- Play a track
- Play an album in reverse

> mplay loop shuffle /path/to/playlist-1 /path/to/playlist-2, track.mp3, reverse /path/to/album

## Picking

Play the first 3 tracks from an album:

> mplay pick-3 /path/to/album

Play the last track from an album:

> mplay pick-1 reverse /path/to/album

Play 10 random tracks from a playlist:

> mplay pick-10 shuffle /path/to/playlist

Shuffle the first 10 tracks of a playlist:

> mplay shuffle pick-10 /path/to/playlist


