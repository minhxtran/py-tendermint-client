# Python Tendermint client (HTTP)

### Install
Requires Python 3.6

Recommend [PipEnv](http://docs.pipenv.org/en/latest/) for a virtualenv but not required
```
git clone https://github.com/davebryson/py-tendermint-client
cd py-tendermint-client
pipenv --three # for a python 3 virtualenv
pipenv install
```

### Try it out
```
In one terminal run the tendermint dummy app
>> dummy

In another terminal run tendermint
>> tendermint node

In another fire up a console
>> python
>>> from tendermint import Tendermint
>>> t = Tendermint()
>>> t.status()
>>> t.broadcast_tx_commit('helloworld')
...
```
