1. #git clone https://github.com/hashicorp/terraform.git - клонироване репозитория на пк
2. #1.PS E:\publik\devops\1402\terraform> git show aefea
3. ##commit aefead2207ef7e2aa5dc81a34aedf0cad4c32545 - полный хеш
4. ##Update CHANGELOG.md
5. 
6. #2.PS E:\publik\devops\1402\terraform> git show 85024d3
7. ##commit 85024d3100126de36331c6982bfaac02cdab9e76 (tag: v0.12.23)
8. ##Author: tf-release-bot <terraform@hashicorp.com>
9.
10. #3.PS E:\publik\Devops\1402\terraform> git show --pretty=format:'%P' b8d720
11. ##56cd7859e05c36c06b56d013b55a252d0bb7e158 
12. ##9ea88f22fc6269854151c571162c5bcf958bee2b
13.
14. #4. PS E:\publik\Devops\1402\terraform> git log v0.12.23..v0.12.24 --pretty=oneline 
15. ##33ff1c03bb960b332be3af2e333462dde88b279e (tag: v0.12.24) v0.12.24
16. ##b14b74c4939dcab573326f4e3ee2a62e23e12f89 [Website] vmc provider links
17. ##3f235065b9347a758efadc92295b540ee0a5e26e Update CHANGELOG.md
18. ##6ae64e247b332925b872447e9ce869657281c2bf registry: Fix panic when server is unreachable
19. ##5c619ca1baf2e21a155fcdb4c264cc9e24a2a353 website: Remove links to the getting started guide's old location
20. ##06275647e2b53d97d4f0a19a0fec11f6d69820b5 Update CHANGELOG.md
21. ##d5f9411f5108260320064349b757f55c09bc4b80 command: Fix bug when using terraform login on Windows
22. ##4b6d06cc5dcb78af637bbb19c198faff37a066ed Update CHANGELOG.md
23. ##dd01a35078f040ca984cdd349f18d0b67e486c35 Update CHANGELOG.md
24. ##225466bc3e5f35baa5d07197bbc079345b77525e Cleanup after v0.12.23 release
25.
26. #5.PS E:\publik\Devops\1402\terraform> git log -S'func providerSource(' --oneline
27. ##8c928e8358 main: Consult local directories as potential mirrors of providers
28. 
28. #6. PS E:\publik\Devops\1402\terraform> git grep 'func globalPluginDirs' - поиск   комита  
29. ##plugins.go:func globalPluginDirs() []string {  - в данный файл были внесены изменения
30. ##PS E:\publik\Devops\1402\terraform> git log  plugins.go          
31. ##commit ffe056bacb9f2cf403fa3b6b894c5fbe1fa850a7
32. ##Author: Martin Atkins <mart@degeneration.co.uk> Date:   Mon May 17 12:07:38 2021 -0700   Move command/ to internal/command/
33. ##commit 78b12205587fe839f10d946ea3fdc06719decb05
34. ##Author: Pam Selle <204372+pselle@users.noreply.github.com> - Remove config.go and update things using its aliases
35. ##commit 52dbf94834cb970b510f2fba853a5b49ad9b1a46 
36. ##Author: James Bardin <j.bardin@gmail.com> -    keep .terraform.d/plugins for discovery
37. ##commit 41ab0aef7a0fe030e84018973a64135b11abcd70
38. ##Author: James Bardin <j.bardin@gmail.com> -   Add missing OS_ARCH dir to global plugin paths
39. ##commit 66ebff90cdfaa6938f26f908c7ebad8d547fea17
40. ##Author: James Bardin <j.bardin@gmail.com> -   move some more plugin search path logic to command
41. ##commit 8364383c359a6b738a436d1b7745ccdce178df47
42. ##Author: Martin Atkins <mart@degeneration.co.uk> - Push plugin discovery down into command package
43. 
43. #7. PS E:\publik\Devops\1402\terraform> git log -S'func synchronizedWriters(' --pretty=format:'%h - %an %ae'
44. ##bdfea50cc8 - James Bardin j.bardin@gmail.com - Date:   Mon Nov 30 18:02:04 2020 -0500
45. ##commit bdfea50cc85161dea41be0fe3381fd98731ff786 -  remove unused
46. ##5ac311e2a9 - Martin Atkins mart@degeneration.co.uk - commit 5ac311e2a91e381e2f52234668b49ba670aa0fe5
47. ##Wed May 3 16:25:41 2017 -0700 . Дата создания более ранняя. Автор
