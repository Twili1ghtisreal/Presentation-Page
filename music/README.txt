Drop your mp3 files in this folder, then list them in index.html — near the top of
the <script>, in the MUSIC array.

The title is taken from the file name (extension removed), so this:

  const MUSIC = [
    "music/My Song, Your Note.mp3",
    "music/another-track.mp3",
  ];

shows up as "My Song, Your Note" and "another-track" in the little toast.

Want a nicer title than the file name? Use the long form:

  { title: "My Song, Your Note", file: "music/My Song, Your Note.mp3" }

The music starts by itself when the page opens. The music note button in the nav opens
a small panel: track name, previous / play-pause / next, and a volume slider.
Tracks advance automatically when one ends, and a single track just loops.
If a visitor pauses it, that's remembered for their next visit.

Keep file names simple — avoid # and ? characters, which cause URL problems.
