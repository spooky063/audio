# Audio

## Prerequis

- wget
- [ffmpeg](https://github.com/FFmpeg/FFmpeg)
- [yt-dlp](https://github.com/yt-dlp/yt-dlp)
- [AtomicParsley](https://github.com/wez/atomicparsley)

## Utilisation

```bash
./audio.sh <commande> [arguments]
```

### Commandes

- `get_chapters <audio_file1.m4a> <audio_file2.m4a>` : Récupére les chapitres de toutes les pistes audio passées en argument
- `adjust_chapters_correctly <metadata_file1.txt> <metadata_file2.txt>` : Ajuste les chapitres pour qu’ils commencent à la bonne place selon l'ordre des pistes audio
- `delete_chapters_from_metadata <metadata_file1.txt> <metadata_file2.txt>` : Supprime les chapitres des fichiers metadata
- `set_chapters <audio_file> <metadata_file>.txt` : Ajoute les chapitres à la nouvelle piste audio
- `prepare_audio_files <audio_file1.m4a> <audio_file2.m4a>` : Prépare le fichier qui liste des pistes audio selon l'ordre d'écoute
- `correct_audio_frequency <audio_file1.m4a> <audio_file2.m4a>` : Corrige la fréquence audio pour qu’elle soit égale à 48000 Hz (si besoin, pour de l'audio 44100 mHz est suffisant)
- `merge_audio` : Fusionne les fichiers audio
- `merge_metadata <metadata_file1.txt> <metadata_file2.txt>` : Prépare le fichier metadata qui liste les chapitres selon l'ordre d'écoute
- `set_thumbnail <audio_file> <cover_path>` : Met le thumbnail sur la nouvelle piste audio