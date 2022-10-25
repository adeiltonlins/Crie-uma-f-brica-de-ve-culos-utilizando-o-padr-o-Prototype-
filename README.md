# Crie-uma-f-brica-de-ve-culos-utilizando-o-padr-o-Prototype-

 /* Abstract CarShop "class" */
    var CarShop = function(){};
    CarShop.prototype = {
     sellCar: function (type, features) {
      var car = this.manufactureCar(type, features);
     
      getMoney(); // make-believe function
     
      r:function(car, eatuecorate chnique laid out in CarFactory onction (type, features
      
      /* Subclass CarShop and create factory method */
    var JoeCarShop = function() {};
    JoeCarShop.prototype = new CarShop();
    JoeCarShop.prototype.manufactureCar = function (type, features) {
     var car;
     
     // Create a different car depending on what type the user specified
     switch(type) {
      case 'sedan':
       car = new JoeSedanCar();
       break;
      case 'hatchback':
       car = new JoeHatchbackCar();
       break;
      case 'coupe':
      default:
       car = new JoeCoupeCar();
     }
     
     // Decorate the car with the specified features
     return this.decorateCar(car, features);
    };
