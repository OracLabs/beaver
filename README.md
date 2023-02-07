<h1>Orac • MLOps for (online) machine learning</h1>

**🚧 The purpose of Orac is to make launching and hosting an end-to-end online machine learning pipeline easy. It is the next generation of 'beaver' and part of the [online machine learning](https://github.com/online-ml) ecosystem. We have a first working sample [here](https://github.com/MaxHalford/taxi-demo-rp-mz-rv-rd-st) and more to come. 

<div align="center" >
  <img src="https://user-images.githubusercontent.com/18452001/214675829-7ef3f6f4-a1dc-41a2-9ce2-7b8cca3eb6df.png" width="40%" align="right" />
</div>

## 👋 Introduction

Orac is...

🍱 [*The whole package*](https://www.youtube.com/watch?v=nzFTmJnIakk&list=PLIU25-FciwNaz5PqWPiHmPCMOFYoEsJ8c&index=5) • it's a framework to develop, deploy, and maintain machine learning models. Including feature engineering.

🤟 *Straightforward* • there's a UI to see stuff, and an API to do stuff.

🍥 *Online-first* • it is designed for online machine learning models, while also supporting batch models.

☝️ *Opinionated* • it encourages you to [process data with SQL](https://www.ethanrosenthal.com/2022/05/10/database-bundling/) and build models in Python.

🔋 *Batteries included* • default infrastructure and monitoring are provided.

🐢 [*Interfaces all the way down*](https://vadosware.io/post/building-an-interface-with-one-implementation-is-unquestionably-right/) • you can plug in your existing message broker, stream processor, model store, etc. At least, that's the idea.

## 🤱 Getting started

The easiest way is to run the provided [`docker-compose.yaml`](docker-compose.yaml) 🐳

```sh
git clone git@github.com:OracLabs/orac.git
cd orac
docker-compose up
```

Go to [http://localhost:3000](http://localhost:3000/) to check out the UI. This is a read-only interface. Interacting with the system happens through an API.

Go to [http://localhost:8080/topics](http://localhost:8080/topics) to see all the kafka topics and their content easily as you run your models.

The recommended next step is to move on to the examples. That will give you an understanding of the workflow which Beaver enables.

## 👀 Examples

- [🚕 Taxis](examples/taxis)

## 📈 Dashboard
Go to [http://localhost:4000/](http://localhost:4000/d/-GzUaVo4z/model-performance-dashboard-sample?orgId=1) to check out the sample Grafana Dashboard included for Taxi demo.

## 🚀 Deployment

The `docker-compose.yaml` file is meant for development. You'll want to edit it if you're looking to deploy Beaver.

## 📝 License

Beaver is free and open-source software licensed under the [3-clause BSD license](LICENSE).
