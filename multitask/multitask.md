| Dataset    | dailydialog | gsm8k | persona-chat | samsum |
|------------|-------------|-------|--------------|--------|
| In-Context | 12.28       | 44.48 | 9.32         | 34.01  |
| Naive      | 7.85        | 24.7  | 8.97         | None   |
| SHINE      | 17.12       | 25.27 | 16.07        | 46.18  |

We fine-tuning the hypernetwork after instructin fine-tuning mqa using these 4 datasets (fine-tuning 4 at the same time, not only fine-tuning one each time). These 4 datasets represent 4 different tasks.
- dailydialog: conversation history to lora.
- gsm8k: reasoning.
- persona-chat: perferences and personality to lora.
- samsum: summarization

SHINE achieve outstanding results on dailydialog, persona-chat and samsum. The only exception is gsm8k, and we think this is because all instruction fine-tuning doesn't contain any reasoning datas and no other skills like reinforcement learning are used to enhance reasoning skills.
