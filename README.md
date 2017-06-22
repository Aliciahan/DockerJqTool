<h1 id="0" align="center">jq for docker</h1>

<h2 id="1">Basic Usage</h2>

~~~bash
docker run --rm --name test jqtool sh -c '/entrypoint.sh'
docker cp ./test.json name:/
docker exec test sh -c "cat /test.json | jq .[1].sports[1]"
docker stop test
~~~
