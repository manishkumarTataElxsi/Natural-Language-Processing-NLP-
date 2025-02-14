# **Speech and Language Processing: An Introduction to Natural Language Processing, Computational Linguistics, and Speech Recognition**

## 1 Introduction 1
1.1 Knowledge in Speech and Language Processing . . . . . . . . . . . 2
1.2 Ambiguity . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4
1.3 Models and Algorithms . . . . . . . . . . . . . . . . . . . . . . . . 5
1.4 Language, Thought, and Understanding . . . . . . . . . . . . . . . . 6
1.5 The State of the Art . . . . . . . . . . . . . . . . . . . . . . . . . . 8
1.6 Some Brief History . . . . . . . . . . . . . . . . . . . . . . . . . . 9
1.6.1 Foundational Insights: 1940s and 1950s . . . . . . . . . . . 9
1.6.2 The Two Camps: 1957–1970 . . . . . . . . . . . . . . . . . 10
1.6.3 Four Paradigms: 1970–1983 . . . . . . . . . . . . . . . . . 11
1.6.4 Empiricism and Finite State Models Redux: 1983–1993 . . 12
1.6.5 The Field Comes Together: 1994–1999 . . . . . . . . . . . 12
1.6.6 The Rise of Machine Learning: 2000–2007 . . . . . . . . . 13
1.6.7 On Multiple Discoveries . . . . . . . . . . . . . . . . . . . 13
1.6.8 A Final Brief Note on Psychology . . . . . . . . . . . . . . 14
1.7 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 15
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 15

# I Words
## 2 Regular Expressions and Automata 17
2.1 Regular Expressions . . . . . . . . . . . . . . . . . . . . . . . . . . 17
2.1.1 Basic Regular Expression Patterns . . . . . . . . . . . . . . 18
2.1.2 Disjunction, Grouping, and Precedence . . . . . . . . . . . 21
2.1.3 A Simple Example . . . . . . . . . . . . . . . . . . . . . . 22
2.1.4 A More Complex Example . . . . . . . . . . . . . . . . . . 23
2.1.5 Advanced Operators . . . . . . . . . . . . . . . . . . . . . 24
2.1.6 Regular Expression Substitution, Memory, and ELIZA . . . 25
2.2 Finite-State Automata . . . . . . . . . . . . . . . . . . . . . . . . . 26
2.2.1 Using an FSA to Recognize Sheeptalk . . . . . . . . . . . . 26
2.2.2 Formal Languages . . . . . . . . . . . . . . . . . . . . . . 30
2.2.3 Another Example . . . . . . . . . . . . . . . . . . . . . . . 31
2.2.4 Non-Deterministic FSAs . . . . . . . . . . . . . . . . . . . 32
2.2.5 Using an NFSA to Accept Strings . . . . . . . . . . . . . . 33
2.2.6 Recognition as Search . . . . . . . . . . . . . . . . . . . . 35
2.2.7 Relating Deterministic and Non-Deterministic Automata . . 38
2.3 Regular Languages and FSAs . . . . . . . . . . . . . . . . . . . . . 38
2.4 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 40
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 42
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 42

## 3 Words & Transducers 45
3.1 Survey of (Mostly) English Morphology . . . . . . . . . . . . . . . 47
3.1.1 Inflectional Morphology . . . . . . . . . . . . . . . . . . . 48
3.1.2 Derivational Morphology . . . . . . . . . . . . . . . . . . . 50
3.1.3 Cliticization . . . . . . . . . . . . . . . . . . . . . . . . . . 51
3.1.4 Non-concatenative Morphology . . . . . . . . . . . . . . . 52
3.1.5 Agreement . . . . . . . . . . . . . . . . . . . . . . . . . . 52
3.2 Finite-State Morphological Parsing . . . . . . . . . . . . . . . . . . 53
3.3 Building a Finite-State Lexicon . . . . . . . . . . . . . . . . . . . . 54
3.4 Finite-State Transducers . . . . . . . . . . . . . . . . . . . . . . . . 57
3.4.1 Sequential Transducers and Determinism . . . . . . . . . . 59
3.5 FSTs for Morphological Parsing . . . . . . . . . . . . . . . . . . . 60
3.6 Transducers and Orthographic Rules . . . . . . . . . . . . . . . . . 63
3.7 Combining FST Lexicon and Rules . . . . . . . . . . . . . . . . . . 65
3.8 Lexicon-Free FSTs: The Porter Stemmer . . . . . . . . . . . . . . . 68
3.9 Word and Sentence Tokenization . . . . . . . . . . . . . . . . . . . 69
3.9.1 Segmentation in Chinese . . . . . . . . . . . . . . . . . . . 70
3.10 Detecting and Correcting Spelling Errors . . . . . . . . . . . . . . . 72
3.11 Minimum Edit Distance . . . . . . . . . . . . . . . . . . . . . . . . 74
3.12 Human Morphological Processing . . . . . . . . . . . . . . . . . . 77
3.13 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 79
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 80
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 81

## 4 N-grams 83
4.1 Counting Words in Corpora . . . . . . . . . . . . . . . . . . . . . . 84
4.2 Simple (Unsmoothed) N-grams . . . . . . . . . . . . . . . . . . . . 86
4.3 Training and Test Sets . . . . . . . . . . . . . . . . . . . . . . . . . 91
4.3.1 N-gram Sensitivity to the Training Corpus . . . . . . . . . . 92
4.3.2 Unknown Words: Open versus closed vocabulary tasks . . . 94
4.4 Evaluating N-grams: Perplexity . . . . . . . . . . . . . . . . . . . . 95
4.5 Smoothing . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 97
4.5.1 Laplace Smoothing . . . . . . . . . . . . . . . . . . . . . . 98
4.5.2 Good-Turing Discounting . . . . . . . . . . . . . . . . . . 101
4.5.3 Some advanced issues in Good-Turing estimation . . . . . . 102
4.6 Interpolation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 103
4.7 Backoff . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 105
4.7.1 Advanced: Details of computing Katz backoff α and P
4.8 Practical Issues: Toolkits and Data Formats . . . . . . . . . . . . . . 107
4.9 Advanced Issues in Language Modeling . . . . . . . . . . . . . . . 109
4.9.1 Advanced Smoothing Methods: Kneser-Ney Smoothing . . 109
4.9.2 Class-based N-grams . . . . . . . . . . . . . . . . . . . . . 111
4.9.3 Language Model Adaptation and Using the Web . . . . . . 111
4.9.4 Using Longer Distance Information: A Brief Summary . . . 112
4.10 Advanced: Information Theory Background . . . . . . . . . . . . . 113
4.10.1 Cross-Entropy for Comparing Models . . . . . . . . . . . . 116
4.11 Advanced: The Entropy of English and Entropy Rate Constancy . . 117
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 119
4.12 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 120
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 121

## 5 Part-of-Speech Tagging 123
5.1 (Mostly) English Word Classes . . . . . . . . . . . . . . . . . . . . 124
5.2 Tagsets for English . . . . . . . . . . . . . . . . . . . . . . . . . . . 130
5.3 Part-of-Speech Tagging . . . . . . . . . . . . . . . . . . . . . . . . 133
5.4 Rule-Based Part-of-Speech Tagging . . . . . . . . . . . . . . . . . . 137
5.5 HMM Part-of-Speech Tagging . . . . . . . . . . . . . . . . . . . . 139
5.5.1 Computing the most-likely tag sequence: An example . . . 142
5.5.2 Formalizing Hidden Markov Model taggers . . . . . . . . . 144
5.5.3 The Viterbi Algorithm for HMM Tagging . . . . . . . . . . 145
5.5.4 Extending the HMM algorithm to trigrams . . . . . . . . . 149
5.6 Transformation-Based Tagging . . . . . . . . . . . . . . . . . . . . 151
5.6.1 How TBL Rules Are Applied . . . . . . . . . . . . . . . . 152
5.6.2 How TBL Rules Are Learned . . . . . . . . . . . . . . . . 152
5.7 Evaluation and Error Analysis . . . . . . . . . . . . . . . . . . . . . 153
5.7.1 Error Analysis . . . . . . . . . . . . . . . . . . . . . . . . 156
5.8 Advanced Issues in Part-of-Speech Tagging . . . . . . . . . . . . . 157
5.8.1 Practical Issues: Tag Indeterminacy and Tokenization . . . . 157
5.8.2 Unknown Words . . . . . . . . . . . . . . . . . . . . . . . 158
5.8.3 Part-of-Speech Tagging for Other Languages . . . . . . . . 160
5.8.4 Combining Taggers . . . . . . . . . . . . . . . . . . . . . . 163
5.9 Advanced: The Noisy Channel Model for Spelling . . . . . . . . . . 163
5.9.1 Contextual Spelling Error Correction . . . . . . . . . . . . 167
5.10 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 168
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 169
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 171

## 6 Hidden Markov and Maximum Entropy Models 173
6.1 Markov Chains . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 174
6.2 The Hidden Markov Model . . . . . . . . . . . . . . . . . . . . . . 177
6.3 Computing Likelihood: The Forward Algorithm . . . . . . . . . . . 179
6.4 Decoding: The Viterbi Algorithm . . . . . . . . . . . . . . . . . . . 184
6.5 Training HMMs: The Forward-Backward Algorithm . . . . . . . . . 187
6.6 Maximum Entropy Models: Background . . . . . . . . . . . . . . . 193
6.6.1 Linear Regression . . . . . . . . . . . . . . . . . . . . . . 194
6.6.2 Logistic regression . . . . . . . . . . . . . . . . . . . . . . 197
6.6.3 Logistic regression: Classification . . . . . . . . . . . . . . 199
6.6.4 Advanced: Learning in logistic regression . . . . . . . . . . 200
6.7 Maximum Entropy Modeling . . . . . . . . . . . . . . . . . . . . . 201
6.7.1 Why do we call it Maximum Entropy? . . . . . . . . . . . . 205
6.8 Maximum Entropy Markov Models . . . . . . . . . . . . . . . . . . 207
6.8.1 Decoding and Learning in MEMMs . . . . . . . . . . . . . 210
6.9 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 212
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 212
# II Speech
## 7 Phonetics 215
7.1 Speech Sounds and Phonetic Transcription . . . . . . . . . . . . . . 216
7.2 Articulatory Phonetics . . . . . . . . . . . . . . . . . . . . . . . . . 218
7.2.1 The Vocal Organs . . . . . . . . . . . . . . . . . . . . . . . 218
7.2.2 Consonants: Place of Articulation . . . . . . . . . . . . . . 220
7.2.3 Consonants: Manner of Articulation . . . . . . . . . . . . . 221
7.2.4 Vowels . . . . . . . . . . . . . . . . . . . . . . . . . . . . 222
7.3 Phonological Categories and Pronunciation Variation . . . . . . . . 225
7.3.1 Phonetic Features . . . . . . . . . . . . . . . . . . . . . . . 227
7.3.2 Predicting Phonetic Variation . . . . . . . . . . . . . . . . 228
7.3.3 Factors Influencing Phonetic Variation . . . . . . . . . . . . 229
7.4 Acoustic Phonetics and Signals . . . . . . . . . . . . . . . . . . . . 230
7.4.1 Waves . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 231
7.4.2 Speech Sound Waves . . . . . . . . . . . . . . . . . . . . . 231
7.4.3 Frequency and Amplitude; Pitch and Loudness . . . . . . . 233
7.4.4 Interpreting Phones from a Waveform . . . . . . . . . . . . 236
7.4.5 Spectra and the Frequency Domain . . . . . . . . . . . . . 236
7.4.6 The Source-Filter Model . . . . . . . . . . . . . . . . . . . 241
7.5 Phonetic Resources . . . . . . . . . . . . . . . . . . . . . . . . . . 241
7.6 Advanced: Articulatory and Gestural Phonology . . . . . . . . . . . 244
7.7 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 245
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 246
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 247

## 8 Speech Synthesis 249
8.1 Text Normalization . . . . . . . . . . . . . . . . . . . . . . . . . . 250
8.1.1 Sentence Tokenization . . . . . . . . . . . . . . . . . . . . 251
8.1.2 Non-Standard Words . . . . . . . . . . . . . . . . . . . . . 253
8.1.3 Homograph Disambiguation . . . . . . . . . . . . . . . . . 256
8.2 Phonetic Analysis . . . . . . . . . . . . . . . . . . . . . . . . . . . 257
8.2.1 Dictionary Lookup . . . . . . . . . . . . . . . . . . . . . . 258
8.2.2 Names . . . . . . . . . . . . . . . . . . . . . . . . . . . . 259
8.2.3 Grapheme-to-Phoneme . . . . . . . . . . . . . . . . . . . . 259
8.3 Prosodic Analysis . . . . . . . . . . . . . . . . . . . . . . . . . . . 263
8.3.1 Prosodic Structure . . . . . . . . . . . . . . . . . . . . . . 263
8.3.2 Prosodic prominence . . . . . . . . . . . . . . . . . . . . . 264
8.3.3 Tune . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 267
8.3.4 More sophisticated models: ToBI . . . . . . . . . . . . . . 267
8.3.5 Computing duration from prosodic labels . . . . . . . . . . 270
8.3.6 Computing F0 from prosodic labels . . . . . . . . . . . . . 271
8.3.7 Final result of text analysis: Internal Representation . . . . 272
8.4 Diphone Waveform synthesis . . . . . . . . . . . . . . . . . . . . . 273
8.4.1 Building a diphone database . . . . . . . . . . . . . . . . . 274
8.4.2 Diphone concatenation and TD-PSOLA for prosody . . . . 275
8.5 Unit Selection (Waveform) Synthesis . . . . . . . . . . . . . . . . . 278
8.6 Evaluation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 282
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 283
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 285

## 9 Automatic Speech Recognition 287
9.1 Speech Recognition Architecture . . . . . . . . . . . . . . . . . . . 289
9.2 Applying the Hidden Markov Model to Speech . . . . . . . . . . . . 293
9.3 Feature Extraction: MFCC vectors . . . . . . . . . . . . . . . . . . 297
9.3.1 Preemphasis . . . . . . . . . . . . . . . . . . . . . . . . . 298
9.3.2 Windowing . . . . . . . . . . . . . . . . . . . . . . . . . . 298
9.3.3 Discrete Fourier Transform . . . . . . . . . . . . . . . . . . 300
9.3.4 Mel filter bank and log . . . . . . . . . . . . . . . . . . . . 301
9.3.5 The Cepstrum: Inverse Discrete Fourier Transform . . . . . 302
9.3.6 Deltas and Energy . . . . . . . . . . . . . . . . . . . . . . 304
9.3.7 Summary: MFCC . . . . . . . . . . . . . . . . . . . . . . 304
9.4 Computing Acoustic Likelihoods . . . . . . . . . . . . . . . . . . . 305
9.4.1 Vector Quantization . . . . . . . . . . . . . . . . . . . . . 305
9.4.2 Gaussian PDFs . . . . . . . . . . . . . . . . . . . . . . . . 308
9.4.3 Probabilities, log probabilities and distance functions . . . . 315
9.5 The Lexicon and Language Model . . . . . . . . . . . . . . . . . . 316
9.6 Search and Decoding . . . . . . . . . . . . . . . . . . . . . . . . . 316
9.7 Embedded Training . . . . . . . . . . . . . . . . . . . . . . . . . . 326
9.8 Evaluation: Word Error Rate . . . . . . . . . . . . . . . . . . . . . 330
9.9 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 332
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 333
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 336

## 10 Speech Recognition: Advanced Topics 337
10.1 Multipass Decoding: N-best lists and lattices . . . . . . . . . . . . . 338
10.2 A∗(‘Stack’) Decoding . . . . . . . . . . . . . . . . . . . . . . . . . 343
10.3 Context-Dependent Acoustic Models: Triphones . . . . . . . . . . . 347
10.4 Discriminative Training . . . . . . . . . . . . . . . . . . . . . . . . 351
10.4.1 Maximum Mutual Information Estimation . . . . . . . . . . 352
10.4.2 Acoustic Models based on Posterior Classifiers . . . . . . . 354
10.5 Modeling Variation . . . . . . . . . . . . . . . . . . . . . . . . . . 355
10.5.1 Environmental Variation and Noise . . . . . . . . . . . . . 355
10.5.2 Speaker and Dialect Adaptation: Variation due to speaker differences . . . . . . . . . . . . . . . . . . . . . . . . . . 356
10.5.3 Pronunciation Modeling: Variation due to Genre . . . . . . 357
10.6 Metadata: Boundaries, Punctuation, and Disfluencies . . . . . . . . 359
10.7 Speech Recognition by Humans . . . . . . . . . . . . . . . . . . . . 361
10.8 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 363
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 363
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 364

## 11 Computational Phonology 365
11.1 Finite-State Phonology . . . . . . . . . . . . . . . . . . . . . . . . 365
11.2 Advanced Finite-State Phonology . . . . . . . . . . . . . . . . . . . 369
11.2.1 Harmony . . . . . . . . . . . . . . . . . . . . . . . . . . . 369
11.2.2 Templatic Morphology . . . . . . . . . . . . . . . . . . . . 370
11.3 Computational Optimality Theory . . . . . . . . . . . . . . . . . . . 371
11.3.1 Finite-State Transducer Models of Optimality Theory . . . . 373
11.3.2 Stochastic Models of Optimality Theory . . . . . . . . . . . 375
11.4 Syllabification . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 376
11.5 Learning Phonology & Morphology . . . . . . . . . . . . . . . . . 380
11.5.1 Learning Phonological Rules . . . . . . . . . . . . . . . . . 380
11.5.2 Learning Morphology . . . . . . . . . . . . . . . . . . . . 381
11.5.3 Learning in Optimality Theory . . . . . . . . . . . . . . . . 385
11.6 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 386
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 386
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 388

# III Syntax
## 12 Formal Grammars of English 389
12.1 Constituency . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 390
12.2 Context-Free Grammars . . . . . . . . . . . . . . . . . . . . . . . . 391
12.2.1 Formal definition of context-free grammar . . . . . . . . . 395
12.3 Some Grammar Rules for English . . . . . . . . . . . . . . . . . . . 396
12.3.1 Sentence-Level Constructions . . . . . . . . . . . . . . . . 396
12.3.2 Clauses and Sentences . . . . . . . . . . . . . . . . . . . . 398
12.3.3 The Noun Phrase . . . . . . . . . . . . . . . . . . . . . . . 398
12.3.4 Agreement . . . . . . . . . . . . . . . . . . . . . . . . . . 403
12.3.5 The Verb Phrase and Subcategorization . . . . . . . . . . . 404
12.3.6 Auxiliaries . . . . . . . . . . . . . . . . . . . . . . . . . . 406
12.3.7 Coordination . . . . . . . . . . . . . . . . . . . . . . . . . 407
12.4 Treebanks . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 408
12.4.1 Example: The Penn Treebank Project . . . . . . . . . . . . 408
12.4.2 Using a Treebank as a Grammar . . . . . . . . . . . . . . . 410
12.4.3 Searching Treebanks . . . . . . . . . . . . . . . . . . . . . 412
12.4.4 Heads and Head Finding . . . . . . . . . . . . . . . . . . . 413
12.5 Grammar Equivalence and Normal Form . . . . . . . . . . . . . . . 416
12.6 Finite-State and Context-Free Grammars . . . . . . . . . . . . . . . 417
12.7 Dependency Grammars . . . . . . . . . . . . . . . . . . . . . . . . 418
12.7.1 The Relationship Between Dependencies and Heads . . . . 419
12.7.2 Categorial Grammar . . . . . . . . . . . . . . . . . . . . . 420
12.8 Spoken Language Syntax . . . . . . . . . . . . . . . . . . . . . . . 421
12.8.1 Disfluencies and Repair . . . . . . . . . . . . . . . . . . . 422
12.8.2 Treebanks for Spoken Language . . . . . . . . . . . . . . . 423
12.9 Grammars and Human Processing . . . . . . . . . . . . . . . . . . . 423
12.10 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 425
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 426
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 428

## 13 Parsing with Context-Free Grammars 431
13.1 Parsing as Search . . . . . . . . . . . . . . . . . . . . . . . . . . . 432
13.1.1 Top-Down Parsing . . . . . . . . . . . . . . . . . . . . . . 433
13.1.2 Bottom-Up Parsing . . . . . . . . . . . . . . . . . . . . . . 434
13.1.3 Comparing Top-Down and Bottom-Up Parsing . . . . . . . 435
13.2 Ambiguity . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 436
13.3 Search in the Face of Ambiguity . . . . . . . . . . . . . . . . . . . 438
13.4 Dynamic Programming Parsing Methods . . . . . . . . . . . . . . . 439
13.4.1 CKY Parsing . . . . . . . . . . . . . . . . . . . . . . . . . 440
13.4.2 The Earley Algorithm . . . . . . . . . . . . . . . . . . . . 447
13.4.3 Chart Parsing . . . . . . . . . . . . . . . . . . . . . . . . . 452
13.5 Partial Parsing . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 454
13.5.1 Finite-State Rule-Based Chunking . . . . . . . . . . . . . . 455
13.5.2 Machine Learning-Based Approaches to Chunking . . . . . 456
13.5.3 Evaluating Chunking Systems . . . . . . . . . . . . . . . . 459
13.6 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 460
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 461
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 462

## 14 Statistical Parsing 465
14.1 Probabilistic Context-Free Grammars . . . . . . . . . . . . . . . . . 466
14.1.1 PCFGs for Disambiguation . . . . . . . . . . . . . . . . . . 467
14.1.2 PCFGs for Language Modeling . . . . . . . . . . . . . . . 469
14.2 Probabilistic CKY Parsing of PCFGs . . . . . . . . . . . . . . . . . 470
14.3 Learning PCFG Rule Probabilities . . . . . . . . . . . . . . . . . . 473
14.4 Problems with PCFGs . . . . . . . . . . . . . . . . . . . . . . . . . 474
14.4.1 Independence assumptions miss structural dependencies between rules . . . . . . . . . . . . . . . . . . . . . . . . . . 474
14.4.2 Lack of sensitivity to lexical dependencies . . . . . . . . . 475
14.5 Improving PCFGs by Splitting and Merging Nonterminals . . . . . . 477
14.6 Probabilistic Lexicalized CFGs . . . . . . . . . . . . . . . . . . . . 479
14.6.1 The Collins Parser . . . . . . . . . . . . . . . . . . . . . . 481
14.6.2 Advanced: Further Details of the Collins Parser . . . . . . . 483
14.7 Evaluating Parsers . . . . . . . . . . . . . . . . . . . . . . . . . . . 485
14.8 Advanced: Discriminative Reranking . . . . . . . . . . . . . . . . . 486
14.9 Advanced: Parser-Based Language Modeling . . . . . . . . . . . . . 488
14.10 Human Parsing . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 489
14.11 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 491
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 492
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 494


## 15 Features and Unification 495
15.1 Feature Structures . . . . . . . . . . . . . . . . . . . . . . . . . . . 496
15.2 Unification of Feature Structures . . . . . . . . . . . . . . . . . . . 499
15.3 Feature Structures in the Grammar . . . . . . . . . . . . . . . . . . 503
15.3.1 Agreement . . . . . . . . . . . . . . . . . . . . . . . . . . 504
15.3.2 Head Features . . . . . . . . . . . . . . . . . . . . . . . . 507
15.3.3 Subcategorization . . . . . . . . . . . . . . . . . . . . . . 508
15.3.4 Long-Distance Dependencies . . . . . . . . . . . . . . . . 513
15.4 Implementing Unification . . . . . . . . . . . . . . . . . . . . . . . 513
15.4.1 Unification Data Structures . . . . . . . . . . . . . . . . . . 514
15.4.2 The Unification Algorithm . . . . . . . . . . . . . . . . . . 515
15.5 Parsing with Unification Constraints . . . . . . . . . . . . . . . . . 519
15.5.1 Integrating Unification into an Earley Parser . . . . . . . . 520
15.5.2 Unification-Based Parsing . . . . . . . . . . . . . . . . . . 526
15.6 Types and Inheritance . . . . . . . . . . . . . . . . . . . . . . . . . 528
15.6.1 Advanced: Extensions to Typing . . . . . . . . . . . . . . 531
15.6.2 Other Extensions to Unification . . . . . . . . . . . . . . . 532
15.7 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 532
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 533
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 534

## 16 Language and Complexity 537
16.1 The Chomsky Hierarchy . . . . . . . . . . . . . . . . . . . . . . . . 538
16.2 How to Tell if a Language Isn’t Regular . . . . . . . . . . . . . . . 540
16.2.1 The Pumping Lemma . . . . . . . . . . . . . . . . . . . . 541
16.2.2 Are English and Other Natural Languages Regular Languages?543
16.3 Is Natural Language Context-Free? . . . . . . . . . . . . . . . . . . 546
16.4 Complexity and Human Processing . . . . . . . . . . . . . . . . . . 548
16.5 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 550
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 551
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 552
# IV Semantics and Pragmatics
## 17 Representing Meaning 553
17.1 Computational Desiderata for Representations . . . . . . . . . . . . 555
17.1.1 Verifiability . . . . . . . . . . . . . . . . . . . . . . . . . . 555
17.1.2 Unambiguous Representations . . . . . . . . . . . . . . . . 556
17.1.3 Canonical Form . . . . . . . . . . . . . . . . . . . . . . . 557
17.1.4 Inference and Variables . . . . . . . . . . . . . . . . . . . . 559
17.1.5 Expressiveness . . . . . . . . . . . . . . . . . . . . . . . . 559
17.2 Model-Theoretic Semantics . . . . . . . . . . . . . . . . . . . . . . 560
17.3 First-Order Logic . . . . . . . . . . . . . . . . . . . . . . . . . . . 563
17.3.1 Basic Elements of First Order Logic . . . . . . . . . . . . . 563
17.3.2 Variables and Quantifiers . . . . . . . . . . . . . . . . . . . 566
17.3.3 Lambda Notation . . . . . . . . . . . . . . . . . . . . . . . 568
17.3.4 The Semantics of First-Order Logic . . . . . . . . . . . . . 569
17.3.5 Inference . . . . . . . . . . . . . . . . . . . . . . . . . . . 570
17.4 Representing Events and States . . . . . . . . . . . . . . . . . . . . 572
17.4.1 Representing Time . . . . . . . . . . . . . . . . . . . . . . 575
17.4.2 Aspect . . . . . . . . . . . . . . . . . . . . . . . . . . . . 578
17.5 Related Representational Approaches . . . . . . . . . . . . . . . . . 581
17.5.1 Description Logics . . . . . . . . . . . . . . . . . . . . . . 582
17.6 Alternative Approaches to Meaning . . . . . . . . . . . . . . . . . . 587
17.6.1 Meaning as Action . . . . . . . . . . . . . . . . . . . . . . 588
17.7 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 588
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 589
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 590

## 18 Computational Semantics 593
18.1 Syntax-Driven Semantic Analysis . . . . . . . . . . . . . . . . . . . 593
18.2 Semantic Augmentations to Context-Free Grammar Rules . . . . . . 595
18.3 Quantifier Scope Ambiguity and Underspecification . . . . . . . . . 602
18.3.1 Store and Retrieve Approaches . . . . . . . . . . . . . . . . 602
18.4 Unification-Based Approaches to Semantic Analysis . . . . . . . . . 604
18.5 Semantic Attachments for a Fragment of English . . . . . . . . . . . 610
18.5.1 Sentences . . . . . . . . . . . . . . . . . . . . . . . . . . . 610
18.5.2 Noun Phrases . . . . . . . . . . . . . . . . . . . . . . . . . 612
18.5.3 Verb Phrases . . . . . . . . . . . . . . . . . . . . . . . . . 615
18.5.4 Prepositional Phrases . . . . . . . . . . . . . . . . . . . . . 617
18.6 Integrating Semantics into the Earley Parser . . . . . . . . . . . . . 619
18.7 Idioms and Compositionality . . . . . . . . . . . . . . . . . . . . . 621
18.8 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 622
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 623
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 624

## 19 Lexical Semantics 627
19.1 Word Senses . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 628
19.2 Relations between Senses . . . . . . . . . . . . . . . . . . . . . . . 631
19.2.1 Synonymy and Antonymy . . . . . . . . . . . . . . . . . . 631
19.2.2 Hyponymy . . . . . . . . . . . . . . . . . . . . . . . . . . 632
19.2.3 Semantic Fields . . . . . . . . . . . . . . . . . . . . . . . . 633
19.3 WordNet: A Database of Lexical Relations . . . . . . . . . . . . . . 633
19.4 Event Participants: Semantic Roles and Selectional Restrictions . . . 635
19.4.1 Thematic Roles . . . . . . . . . . . . . . . . . . . . . . . . 636
19.4.2 Diathesis Alternations . . . . . . . . . . . . . . . . . . . . 637
19.4.3 Problems with Thematic Roles . . . . . . . . . . . . . . . . 639
19.4.4 The Proposition Bank . . . . . . . . . . . . . . . . . . . . 640
19.4.5 FrameNet . . . . . . . . . . . . . . . . . . . . . . . . . . . 641
19.4.6 Selectional Restrictions . . . . . . . . . . . . . . . . . . . 643
19.5 Primitive Decomposition . . . . . . . . . . . . . . . . . . . . . . . 645
19.6 Advanced concepts: Metaphor . . . . . . . . . . . . . . . . . . . . 647
19.7 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 648
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 649
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 650

## 20 Computational Lexical Semantics 653
20.1 Word Sense Disambiguation: Overview . . . . . . . . . . . . . . . . 654
20.2 Supervised Word Sense Disambiguation . . . . . . . . . . . . . . . 655
20.2.1 Extracting Feature Vectors for Supervised Learning . . . . . 656
20.2.2 Naive Bayes and Decision List Classifiers . . . . . . . . . . 657
20.3 WSD Evaluation, Baselines, and Ceilings . . . . . . . . . . . . . . . 660
20.4 WSD: Dictionary and Thesaurus Methods . . . . . . . . . . . . . . 662
20.4.1 The Lesk Algorithm . . . . . . . . . . . . . . . . . . . . . 662
20.4.2 Selectional Restrictions and Selectional Preferences . . . . 664
20.5 Minimally Supervised WSD: Bootstrapping . . . . . . . . . . . . . 666
20.6 Word Similarity: Thesaurus Methods . . . . . . . . . . . . . . . . . 668
20.7 Word Similarity: Distributional Methods . . . . . . . . . . . . . . . 674
20.7.1 Defining a Word’s Co-occurrence Vectors . . . . . . . . . . 675
20.7.2 Measures of Association with Context . . . . . . . . . . . . 676
20.7.3 Defining similarity between two vectors . . . . . . . . . . . 679
20.7.4 Evaluating Distributional Word Similarity . . . . . . . . . . 683
20.8 Hyponymy and other word relations . . . . . . . . . . . . . . . . . 684
20.9 Semantic Role Labeling . . . . . . . . . . . . . . . . . . . . . . . . 687
20.10 Advanced: Unsupervised Sense Disambiguation . . . . . . . . . . . 690
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 691
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 695

## 21 Computational Discourse 697
21.1 Discourse Segmentation . . . . . . . . . . . . . . . . . . . . . . . . 700
21.1.1 Unsupervised Discourse Segmentation . . . . . . . . . . . 700
21.1.2 Supervised Discourse Segmentation . . . . . . . . . . . . . 702
21.1.3 Evaluating Discourse Segmentation . . . . . . . . . . . . . 704
21.2 Text Coherence . . . . . . . . . . . . . . . . . . . . . . . . . . . . 705
21.2.1 Rhetorical Structure Theory . . . . . . . . . . . . . . . . . 706
21.2.2 Automatic Coherence Assignment . . . . . . . . . . . . . . 708
21.3 Reference Resolution . . . . . . . . . . . . . . . . . . . . . . . . . 711
21.4 Reference Phenomena . . . . . . . . . . . . . . . . . . . . . . . . . 714
21.4.1 Five Types of Referring Expressions . . . . . . . . . . . . . 714
21.4.2 Information Status . . . . . . . . . . . . . . . . . . . . . . 716
21.5 Features for Pronominal Anaphora Resolution . . . . . . . . . . . . 717
21.6 Three algorithms for pronominal anaphora resolution . . . . . . . . 720
21.6.1 Pronominal Anaphora Baseline: The Hobbs Algorithm . . 720
21.6.2 A Centering Algorithm for Anaphora Resolution . . . . . . 722
21.6.3 A Log-Linear model for Pronominal Anaphora Resoluton . 724
21.6.4 Features . . . . . . . . . . . . . . . . . . . . . . . . . . . . 725
21.7 Coreference Resolution . . . . . . . . . . . . . . . . . . . . . . . . 726
21.8 Evaluating Coreference Resolution . . . . . . . . . . . . . . . . . . 728
21.9 Advanced: Inference-Based Coherence Resolution . . . . . . . . . . 728
21.10 Psycholinguistic Studies of Reference and Coherence . . . . . . . . 734
21.11 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 735
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 736
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 738

# V Applications
## 22 Information Extraction 741
22.1 Named Entity Recognition . . . . . . . . . . . . . . . . . . . . . . 743
22.1.1 Ambiguity in Named Entity Recognition . . . . . . . . . . 745
22.1.2 NER as Sequence Labeling . . . . . . . . . . . . . . . . . 745
22.1.3 Evaluating Named Entity Recognition . . . . . . . . . . . . 749
22.1.4 Practical NER Architectures . . . . . . . . . . . . . . . . . 750
22.2 Relation Detection and Classification . . . . . . . . . . . . . . . . . 751
22.2.1 Supervised Learning Approaches to Relation Analysis . . . 752
22.2.2 Lightly Supervised Approaches to Relation Analysis . . . . 755
22.2.3 Evaluating Relation Analysis Systems . . . . . . . . . . . . 758
22.3 Temporal and Event Processing . . . . . . . . . . . . . . . . . . . . 759
22.3.1 Temporal Expression Recognition . . . . . . . . . . . . . . 760
22.3.2 Temporal Normalization . . . . . . . . . . . . . . . . . . . 762
22.3.3 Event Detection and Analysis . . . . . . . . . . . . . . . . 765
22.3.4 TimeBank . . . . . . . . . . . . . . . . . . . . . . . . . . . 766
22.4 Template-Filling . . . . . . . . . . . . . . . . . . . . . . . . . . . . 768
22.4.1 Statistical Approaches to Template-Filling . . . . . . . . . 769
22.4.2 Finite-State Template-Filling Systems . . . . . . . . . . . . 770
22.5 Advanced: Biomedical Information Extraction ∗
22.5.1 Biological Named Entity Recognition . . . . . . . . . . . . 774
22.5.2 Gene Normalization . . . . . . . . . . . . . . . . . . . . . 775
22.5.3 Biological Roles and Relations . . . . . . . . . . . . . . . . 776
22.6 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 778
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 778
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 779

## 23 Question Answering and Summarization 783
23.1 Information Retrieval . . . . . . . . . . . . . . . . . . . . . . . . . 785
23.1.1 The Vector Space Model . . . . . . . . . . . . . . . . . . . 786
23.1.2 Term Weighting . . . . . . . . . . . . . . . . . . . . . . . 789
23.1.3 Term Selection and Creation . . . . . . . . . . . . . . . . . 790
23.1.4 Evaluating Information Retrieval Systems . . . . . . . . . . 790
23.1.5 Homonymy, Polysemy, and Synonymy . . . . . . . . . . . 794
23.1.6 Improving User Queries . . . . . . . . . . . . . . . . . . . 795
23.2 Factoid Question Answering . . . . . . . . . . . . . . . . . . . . . 796
23.2.1 Question Processing . . . . . . . . . . . . . . . . . . . . . 798
23.2.2 Passage Retrieval . . . . . . . . . . . . . . . . . . . . . . . 801
23.2.3 Answer Processing . . . . . . . . . . . . . . . . . . . . . . 802
23.2.4 Evaluation of Factoid Answers . . . . . . . . . . . . . . . . 805
23.3 Summarization . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 805
23.3.1 Summarizing Single Documents . . . . . . . . . . . . . . . 808
23.4 Multi-Document Summarization . . . . . . . . . . . . . . . . . . . 814
23.4.1 Content Selection in Multi-Document Summarization . . . 815
23.4.2 Information Ordering in Multi-Document Summarization . 816
23.5 Between Question Answering and Summarization: Query-Focused
Summarization . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 819
23.6 Summarization Evaluation . . . . . . . . . . . . . . . . . . . . . . . 823
23.7 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 825
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 826
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 828

## 24 Dialogue and Conversational Agents 829
24.1 Properties of Human Conversations . . . . . . . . . . . . . . . . . . 831
24.1.1 Turns and Turn-Taking . . . . . . . . . . . . . . . . . . . . 832
24.1.2 Language as Action: Speech Acts . . . . . . . . . . . . . . 833
24.1.3 Language as Joint Action: Grounding . . . . . . . . . . . . 834
24.1.4 Conversational Structure . . . . . . . . . . . . . . . . . . . 836
24.1.5 Conversational Implicature . . . . . . . . . . . . . . . . . . 837
24.2 Basic Dialogue Systems . . . . . . . . . . . . . . . . . . . . . . . . 839
24.2.1 ASR component . . . . . . . . . . . . . . . . . . . . . . . 839
24.2.2 NLU component . . . . . . . . . . . . . . . . . . . . . . . 841
24.2.3 Generation and TTS components . . . . . . . . . . . . . . 844
24.2.4 Dialogue Manager . . . . . . . . . . . . . . . . . . . . . . 845
24.2.5 Dialogue Manager Error Handling: Confirmation/Rejection 849
24.3 VoiceXML . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 851
24.4 Dialogue System Design and Evaluation . . . . . . . . . . . . . . . 854
24.4.1 Designing Dialogue Systems . . . . . . . . . . . . . . . . . 854
24.4.2 Dialogue System Evaluation . . . . . . . . . . . . . . . . . 855
24.5 Information-state & Dialogue Acts . . . . . . . . . . . . . . . . . . 857
24.5.1 Dialogue Acts . . . . . . . . . . . . . . . . . . . . . . . . 859
24.5.2 Interpreting Dialogue Acts . . . . . . . . . . . . . . . . . . 860
24.5.3 Detecting Correction Acts . . . . . . . . . . . . . . . . . . 862
24.5.4 Generating Dialogue Acts: Confirmation and Rejection . . . 863
24.6 Markov Decision Process Architecture . . . . . . . . . . . . . . . . 865
24.7 Advanced: Plan-based Dialogue Agents . . . . . . . . . . . . . . . 869
24.7.1 Plan-Inferential Interpretation and Production . . . . . . . . 869
24.7.2 The Intentional Structure of Dialogue . . . . . . . . . . . . 872
24.8 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 874
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 875
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 876

## 25 Machine Translation 879
25.1 Why is Machine Translation So Hard? . . . . . . . . . . . . . . . . 882
25.1.1 Typology . . . . . . . . . . . . . . . . . . . . . . . . . . . 882
25.1.2 Other Structural Divergences . . . . . . . . . . . . . . . . . 885
25.1.3 Lexical Divergences . . . . . . . . . . . . . . . . . . . . . 885
25.2 Classical MT & the Vauquois Triangle . . . . . . . . . . . . . . . . 887
25.2.1 Direct Translation . . . . . . . . . . . . . . . . . . . . . . 887
25.2.2 Transfer . . . . . . . . . . . . . . . . . . . . . . . . . . . . 890
25.2.3 Combining direct and tranfer approaches in classic MT . . . 892
25.2.4 The Interlingua Idea: Using Meaning . . . . . . . . . . . . 893
25.3 Statistical MT . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 895
25.4 P(F|E): the Phrase-Based Translation Model . . . . . . . . . . . . . 897
25.5 Alignment in MT . . . . . . . . . . . . . . . . . . . . . . . . . . . 900
25.5.1 IBM Model 1 . . . . . . . . . . . . . . . . . . . . . . . . . 901
25.5.2 HMM Alignment . . . . . . . . . . . . . . . . . . . . . . . 903
25.6 Training Alignment Models . . . . . . . . . . . . . . . . . . . . . . 905
25.6.1 EM for Training Alignment Models . . . . . . . . . . . . . 906
25.7 Symmetrizing Alignments for Phrase-based MT . . . . . . . . . . . 908
25.8 Decoding for Phrase-Based Statistical MT . . . . . . . . . . . . . . 910
25.9 MT Evaluation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 914
25.9.1 Using Human Raters . . . . . . . . . . . . . . . . . . . . . 915
25.9.2 Automatic Evaluation: Bleu . . . . . . . . . . . . . . . . . 915
25.10 Advanced: Syntactic Models for MT . . . . . . . . . . . . . . . . . 918
25.11 Advanced: IBM Model 3 for fertility-based alignment . . . . . . . . 920
25.11.1 Training for Model 3 . . . . . . . . . . . . . . . . . . . . . 923
25.12 Advanced: Log-linear Models for MT . . . . . . . . . . . . . . . . 924
Bibliographical and Historical Notes . . . . . . . . . . . . . . . . . . . . . 925
Exercises . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 
