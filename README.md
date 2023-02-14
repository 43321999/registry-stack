# registry-stack
>
>```mermaid
>sequenceDiagram
>    usr->>+dzen: как расшарить реджистри в кластере сворм ?
>    dzen->>+usr: clck.ru/33YFxM
>```
>
setup [nextcloud](https://docs.docker.com/samples/nextcloud/) before: 
## nextcloud service
[43321999/nextcloud-stack](https://github.com/43321999/nextcloud-stack)

```sh
	# registry service
	mkdir -p ~/apps/registry && cd $_
	wget https://github.com/43321999/registry-stack/blob/b8fc3cdb6954d266d20ae100061b6c9533d3c0e4/apps/registry-stack.yml

	docker stack deploy -c registry-stack.yml .
```
```# cat ~/apps/registry-stack.yml:```