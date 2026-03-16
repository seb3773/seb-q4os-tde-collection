---
trigger: always_on
alwaysApply: true
---
# TQt3/Trinity Desktop Standards v2.0

## Knowledge Base (384 classes, 5430 methods)
Use endpoints from manifest.json:
- get_class_detail [CLASSNAME]
- get_method_detail [CLASSNAME] [METHODNAME] 
- search_methods "[PATTERN]"
- get_examples [CLASSNAME]
- get_signals [CLASSNAME]
- get_slots [CLASSNAME]

## Strict Rules
- TQt3 APIs ONLY from KB. Cite source: "From get_class_detail TQWidget"
- No Qt4/5 APIs. No modern C++ beyond C++98
- TQApplication/TQWidget base pattern mandatory
- Memory: TQObject::deleteLater() for children
- Signals/slots: Exact signatures from KB

## Code Template
```cpp
#include <tqapplication.h>
// Other TQt3 includes from KB

int main(int argc, char **argv) {
    TQApplication app(argc, argv);
    // KB-based widget code
    return app.exec();
}

