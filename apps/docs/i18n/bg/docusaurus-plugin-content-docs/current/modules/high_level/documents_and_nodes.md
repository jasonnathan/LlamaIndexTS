---
sidebar_position: 0
---

`Тази документация е преведена автоматично и може да съдържа грешки. Не се колебайте да отворите Pull Request, за да предложите промени.`

# Документи и Възли

`Документи` и `Възли` са основните строителни блокове на всяко индексиране. Въпреки че API-то за тези обекти е подобно, обектите `Документ` представляват цели файлове, докато `Възли` са по-малки части от оригиналния документ, които са подходящи за LLM и Q&A.

```typescript
import { Document } from "llamaindex";

document = new Document({ text: "текст", metadata: { key: "val" } });
```

## API Референция

- [Документ](../../api/classes/Document.md)
- [ТекстовВъзел](../../api/classes/TextNode.md)

"