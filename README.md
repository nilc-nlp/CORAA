# CORAA-v1.1

CORAA is a public available dataset for Automatic Speech Recognition (ASR) in the Brazilian Portuguese language containing 289 hours of audios and their respective transcriptions (400k+ segmented audios). The dataset is composed of audios of 5 original projects:

- ALIP (Gonçalves, 2019)
- C-ORAL Brazil (Raso and Mello, 2012)
- NURC-Recife (Oliviera Jr., 2016)
- SP-2010 (Mendes and Oushiro, 2012)
- TEDx talks (talks in Portuguese)

The audios were either validated by annotators or transcripted for the first time aiming at the ASR task.

## Metadata

- file_path: the path to an audio file
- task: transcription (annotators revised original transcriptions); annotation (annotators classified the audio-transcription pair according to votes_for_* metrics); annotation_and_transcription (both tasks were performed)
- variety: European Portuguese (PT_PT) or Brazilian Portuguese (PT_BR)
- dataset: one of five datasets (ALIP, C-oral Brasil, NURC-RE, SP2010, TEDx Portuguese)
- accent: one of four accents (Minas Gerais, Recife, Sao Paulo cities, Sao Paulo capital) or the value "miscellaneous"
- speech_genre: Interviews, Dialogues, Monologues, Conversations, Interviews, Conference, Class Talks, Stage Talks or Reading
- speech_style: Spontaneous Speech or Prepared Speech or Read Speech
- up_votes: for annotation, the number of votes to valid the audio (most audios were revewed by one annotor, but some of the audios were analyzed by more than one).
- down_votes: for annotation, the number of votes do invalid the audio (always smaller than up_votes)
- votes_for_hesitation: for annotation, votes categorizing the audio as having the hesitation phenomenon
- votes_for_filled_pause: for annotation, votes categorizing the audio as having the filled pause phenomenon
- votes_for_noise_or_low_voice: for annotation, votes categorizing the audio as either having noise or low voice, without impairing the audio compression.
- votes_for_second_voice: for annotation, votes categorizing the audio as having a second voice, without impairing the audio compression
- votes_for_no_identified_problem: without impairing the audio as having no identified phenomenon (of the four described above)
- text: the transcription for the audio

## Downloads : 

Dataset:

- [Train audios](https://drive.google.com/file/d/1deCciFD35EA_OEUl0MrEDa7u5O2KgVJM/view?usp=sharing)
- [Train transcriptions and metadata](https://drive.google.com/file/d/1HbwahfMWoArYj0z2PfI4dHiambWfaNWg/view?usp=sharing)
- [Dev audios](https://drive.google.com/file/d/1bIHctanQjW2ITOM5wNQSt_NjB45s0_Q_/view?usp=sharing)
- [Dev transcriptions and metadata](https://drive.google.com/file/d/185erjax7lS_YNuolZvcMt_EdprafyMU0/view?usp=sharing)
- Test audios (to be released in the future)
- Test transcriptions and metadata (to be released in the future)

Experiments:

- [Checkpoints ](https://drive.google.com/drive/folders/10JkbCzYypZtCz1nHY5rBoBM1r66P3p3j?usp=sharing)
- [Code](https://github.com/Edresson/Wav2Vec-Wrapper)

Model trained in this corpus: Wav2Vec 2.0 XLSR-53 (multilingual pretraining)

## Citation

- [Preprint](https://arxiv.org/abs/2110.15731): 
```
@misc{c2021coraa,
    title={CORAA: a large corpus of spontaneous and prepared speech manually validated for speech recognition in Brazilian Portuguese},
    author={Arnaldo Candido Junior and Edresson Casanova and Anderson Soares and Frederico Santos de Oliveira and Lucas Oliveira and Ricardo Corso Fernandes Junior and Daniel Peixoto Pinto da Silva and Fernando Gorgulho Fayet and Bruno Baldissera Carlotto and Lucas Rafael Stefanel Gris and Sandra Maria Aluísio},
    year={2021},
    eprint={2110.15731},
    archivePrefix={arXiv},
    primaryClass={cs.CL}
}
```

- Full Paper: coming soon
- Oficial site: [Tarsila Project](https://sites.google.com/view/tarsila-c4ai/)

## Partners / Sponsors / Funding

- [C4AI](https://c4ai.inova.usp.br/pt/home-2/)
- [CEIA](https://centrodeia.org/)
- [UFG](https://www.ufg.br/)
- [USP](https://www5.usp.br/)
- [UTFPR](http://www.utfpr.edu.br/)

## References

- Gonçalves SCL (2019) Projeto ALIP (amostra linguística do interior paulista) e banco de dados iboruna: 10 anos de contribuição com a descrição do Português Brasileiro. Revista Estudos Linguísticos 48(1):276–297.
- Raso T, Mello H, Mittmann MM (2012) The C-ORAL-BRASIL I: Reference corpus for spoken Brazilian Portuguese. In: Proceedings of the Eighth International Conference on Language Resources and Evaluation (LREC’12), European Language Resources Association (ELRA), Istanbul, Turkey, pp 106–113, URL http://www.lrec-conf.org/proceedings/lrec2012/pdf/624_Paper.pdf
- Oliviera Jr M (2016) Nurc digital um protocolo para a digitalização, anotação, arquivamento e disseminação do material do projeto da norma urbana linguística culta (NURC). CHIMERA: Revista de Corpus de Lenguas Romances y Estudios Linguísticos 3(2):149–174, URL https://revistas.uam.es/chimera/article/view/6519
- Mendes RB, Oushiro L (2012) Mapping Paulistano Portuguese: the SP2010 Project. In: Proceedings of the VIIth GSCP International Conference: Speech and Corpora, Fizenze University Press, Firenze, Italy, pp 459–463.
