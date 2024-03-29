### Найдите полный хеш и комментарий коммита, хеш которого начинается на aefea.
* aefead2207ef7e2aa5dc81a34aedf0cad4c32545   Update CHANGELOG.md
* git show aefea

### Какому тегу соответствует коммит 85024d3?
* commit 85024d3100126de36331c6982bfaac02cdab9e76 (tag: v0.12.23)
* git show 85024d3

### Сколько родителей у коммита b8d720? Напишите их хеши.
* 2 родителя 56cd7859e05c36c06b56d013b55a252d0bb7e158 9ea88f22fc6269854151c571162c5bcf958bee2b
* git log b8d720 --pretty=format:"%H, %P, %an, %s" --graph

### Перечислите хеши и комментарии всех коммитов, которые были сделаны между тегами v0.12.23 и v0.12.24.
* b14b74c4939dcab573326f4e3ee2a62e23e12f89, [Website] vmc provider links
* 3f235065b9347a758efadc92295b540ee0a5e26e, Update CHANGELOG.md
* 6ae64e247b332925b872447e9ce869657281c2bf, registry: Fix panic when server is unreachable
* 5c619ca1baf2e21a155fcdb4c264cc9e24a2a353, website: Remove links to the getting started guide's old location
* 06275647e2b53d97d4f0a19a0fec11f6d69820b5, Update CHANGELOG.md
* d5f9411f5108260320064349b757f55c09bc4b80, command: Fix bug when using terraform login on Windows
* 4b6d06cc5dcb78af637bbb19c198faff37a066ed, Update CHANGELOG.md
* dd01a35078f040ca984cdd349f18d0b67e486c35, Update CHANGELOG.md
* 225466bc3e5f35baa5d07197bbc079345b77525e, Cleanup after v0.12.23 release
* git log v0.12.23..v0.12.24
* или git log v0.12.24 --pretty=format:"%H, %an, %s" --graph


### Найдите коммит, в котором была создана функция func providerSource, её определение в коде выглядит так: func providerSource(...)
* commit 5af1e6234ab6da412fb8637393c5a17a1b293663
* Author: Martin Atkins <mart@degeneration.co.uk>
* Date:   Tue Apr 21 16:28:59 2020 -0700
* main: Honor explicit provider_installation CLI config when present
* git log -S"func providerSource"

### Найдите все коммиты, в которых была изменена функция globalPluginDirs.
* commit 78b12205587fe839f10d946ea3fdc06719decb05
* commit 52dbf94834cb970b510f2fba853a5b49ad9b1a46
* commit 41ab0aef7a0fe030e84018973a64135b11abcd70
* commit 66ebff90cdfaa6938f26f908c7ebad8d547fea17
* git log -S"func globalPluginDirs"
* и git log -L:"func globalPluginDirs":plugins.go

### Кто автор функции synchronizedWriters?
* Author: Martin Atkins <mart@degeneration.co.uk
* git log -S"func synchronizedWriters"

