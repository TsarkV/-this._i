#Ticker

##Почему this._i не увеличивается. Как исправить?

function Ticker() {
this._i = 0
};
Ticker.prototype = {
 tick: function() {
 console.log(this._i++);
 }
};
var ticker = new Ticker();
setInterval(ticker.tick, 1000);

##Решение
Решение выполнено на javascript. С помощью setTimeout организована остановка увелечения this._i
