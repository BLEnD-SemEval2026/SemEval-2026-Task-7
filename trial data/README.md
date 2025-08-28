# SemEval-2026 Task 7: Everyday Knowledge Accross Diverse Languages and Cultures Trial Data



This README file describes the datasets *trial_data_multiple_choice.tsv* and *trial_data_unique_answer.tsv*, 
provided as trial data for the SemEval-2026 Task 7: Everyday Knowledge Across Diverse Languages and Cultures.



## trial_data_multiple_choice.tsv

This file contains the trial data with multiple-choice options.

### Columns:

- **index**: Data point index.

- **lang_reg**: Language and region code.

- The mapping between the codes and the full language-country names is as follows:

| Code   | Language – Region            |
|--------|------------------------------|
| msa-SG | Malay (Singapore)            |
| tam-SG | Tamil (Singapore)            |
| zho-SG | Chinese (Singapore)          |
| spa-EC | Spanish (Ecuador)            |
| eng-GB | English (United Kingdom)     |
| zho-CN | Chinese (China)              |
| spa-ES | Spanish (Spain)              |
| spa-MX | Spanish (Mexico)             |
| ind-ID | Indonesian (Indonesia)       |
| kor-KR | Korean (South Korea)         |
| ell-GR | Greek (Greece)               |
| fas-IR | Persian/Farsi (Iran)         |
| ara-EG | Arabic (Egypt)               |
| ara-MA | Arabic (Morocco)             |
| ara-SA | Arabic (Saudi Arabia)        |
| eng-AU | English (Australia)          |
| eus-ES | Basque (Spain – Basque Country) |
| fra-FR | French (France)              |
| gle-IE | Irish (Ireland)              |
| tam-LK | Tamil (Sri Lanka)            |
| tgl-PH | Tagalog (Philippines)        |
| bul-BG | Bulgarian (Bulgaria)         |
| jpn-JP | Japanese (Japan)             |

- **question**: The question text.

- **multiple_choice_option**s: The multiple-choice options for the question. Newline characters separate individual options. 

- **correct_answer**: The correct answer to the question. Leading and trailing whitespace has been removed from this column.


 ## trial_data_unique_answer.tsv

- This file contains the trial data with only the correct answer, excluding the multiple-choice options.

### Columns:

- **index**: Data point index

- **lang_reg**: Language and region code.

- The mapping between the codes and the full language-country names is as follows:

| Code   | Language – Region               |
|--------|---------------------------------|
| msa-SG | Malay (Singapore)               |
| tam-SG | Tamil (Singapore)               |
| zho-SG | Chinese (Singapore)             |
| spa-EC | Spanish (Ecuador)               |
| eng-GB | English (United Kingdom)        |
| zho-CN | Chinese (China)                 |
| spa-ES | Spanish (Spain)                 |
| spa-MX | Spanish (Mexico)                |
| ind-ID | Indonesian (Indonesia)          |
| kor-KR | Korean (South Korea)            |
| ell-GR | Greek (Greece)                  |
| fas-IR | Persian/Farsi (Iran)            |
| ara-EG | Arabic (Egypt)                  |
| ara-MA | Arabic (Morocco)                |
| ara-SA | Arabic (Saudi Arabia)           |
| eng-AU | English (Australia)             |
| eus-ES | Basque (Spain – Basque Country) |
| fra-FR | French (France)                 |
| gle-IE | Irish (Ireland)                 |
| tam-LK | Tamil (Sri Lanka)               |
| tgl-PH | Tagalog (Philippines)           |
| bul-BG | Bulgarian (Bulgaria)            |
| jpn-JP | Japanese (Japan)                |

- **question**: The question text.

- **correct_answer**: The correct answer to the question.
