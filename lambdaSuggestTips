exports.handler = (event, context, callback) => {
    //const gender=event.gender;
    const coffee= event.coffee;
    const coffeeAmount = event.coffeeAmount;
    //const city = event.city;
    //const cityDisturbed = event.cityDisturbed;
   // const thirtyMinsBefore= [{activity:"read",ranking: -5},{activity:"screen",ranking:7},{activity:"food", ranking:6},{activity:"drinkWater", ranking:-3},{activity:"drinkOther", ranking:7}, {activity:"socialMedia",ranking:8}, {activity:"domesticActivity", ranking:0}, {activity:"smoke", ranking:10}, {activity:"packBag",ranking:0}];
    //const userThirtyMinsBefore=event.thirtyMins[3]; //make sure you insert 3 and no less 
    //const activity = event.activity;
    //const overallSleepRating=0;
    const pain=event.pain;
    const canSleep = event.canSleep;
    const tips = [{tip:"Drink water before bed", id:"coffee"},{tip:"Please switch off or turn to silent all screen based devices", id:"screen"},{tip:"If you have shoulder pain, try sleeping on your right hand side tonight with your arms at your sides", id:"shoulderPain"}, {tip:"Ask me to play Jane Tepley's meditation set", id:"noSleep"}];
    var result="";
    var coffeeResult="";
    var painResult="";
    var noSleepResult="";
    
    
    if(coffee==='true' && event.coffeeAmount>1){
        
       coffeeResult = tips[tips.findIndex(x => x.id === 'coffee')].tip;
       result=coffeeResult;
    }

    else if(canSleep === 'false'){
       
        noSleepResult=tips[tips.findIndex(x => x.id === 'noSleep')].tip;
        result=noSleepResult;
    }
       else if(pain==='true'){
        
        painResult=tips[tips.findIndex(x => x.id === 'shoulderPain')].tip;
        result=painResult;
    }
    //if(userThirtyMinsBefore.contains("screen")){
   //     tipResult=tips[tips.findIndex(x => x.id === 'screen')].tip;
   // }
    

 
  
    callback(null, result);
};
