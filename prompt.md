Create a landscape A4 PDF guitar fretboard diagram for the [KEY] major scale, frets 0 to 15, using ReportLab (Python).

Layout:
- Six horizontal strings, drawn top to bottom as high e, B, G, D, A, low E. Open-string pitch classes: E=4, B=11, G=7, D=2, A=9, E=4 (C=0).
- Vertical fret lines for frets 0 to 15. The nut (fret 0) is a thicker line. Fret 0 is drawn as an open-string column to the left of the nut, and fret n is centred between fret lines n-1 and n.
- Gray dots at frets 3, 5, 7, 9 and 15 on the middle string. Double dots at fret 12 on the outer strings.
- Fret numbers 1 to 15 below the bottom string. String names in the left margin.
- Title "[KEY] major scale on the guitar fretboard" and a subtitle with the fret range and the page's label mode.
- A legend at the bottom with three entries: root, third and fifth, other scale tones.

Notes:
- Scale tones: a fretted position is a scale tone when (pitch class - root pitch class) mod 12 is in {0, 2, 4, 5, 7, 9, 11}. Those degrees are 1, 2, 3, 4, 5, 6, 7.
- Root colour: #185FA5 (blue). Third and fifth colour: #0F6E56 (teal). Other scale tones: #5F5E5A (gray). Dots and gridlines: #D3D1C7 and #888780.
- Each fret marker is a filled circle of radius 15 with white bold 12pt text.
- Page 1 labels markers with note names (sharps for C#, D#, F#, G#, A#). Page 2 labels markers with scale degrees 1 to 7 instead.
- Root pitch classes: A=9, D=2. Use relative = (pitch class - root) mod 12 when mapping to degrees.
- Save as [key]_major_fretboard_landscape.pdf in the working directory, set the PDF title, and keep both pages in one file.

Verify by rendering the PDF to an image and checking that the root positions and the chosen degrees are correct.
