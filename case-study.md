### 1.1 `Gemfile`

fixed some paths in `Gemfile` as they were outdated

### 2 Algolia

Created an account and configured keys, no issues occurred

## 3. NewRelic

Set up NewRelic, everything was configured quickly and easily with the gem

## 4. Skylight

Set up Skylight, everything went smoothly

## 5. Prometheus + Grafana

Had to tinker a bit since I hadn't worked much with docker and it has its own quirks

## 6. rack-mini-profiler

had already connected it before, no issues occurred

## 7. local_production

## 8. Checked via new relic and skylight and StoriesController#index indeed turned out to be the slowest

initial loading speed was:

[<img src="https://i.ibb.co/mFbQfLD/2021-05-15-20-06.png">](https://i.ibb.co/mFbQfLD/2021-05-15-20-06.png/)
[<img src="https://i.ibb.co/yqkKNHs/2021-05-15-19-47-1.png">](https://i.ibb.co/yqkKNHs/2021-05-15-19-47-1.png/)

After caching the problematic partial, the time was reduced to:
[<img src="https://i.ibb.co/P6FGSsj/2021-05-15-20-10.png">](https://i.ibb.co/P6FGSsj/2021-05-15-20-10.png/)
[<img src="https://i.ibb.co/M9ptzWr/2021-05-15-19-54.png">](https://i.ibb.co/M9ptzWr/2021-05-15-19-54.png)

didn't use touch: true since counter_culture is used in the project

Didn't have time for the bonus
