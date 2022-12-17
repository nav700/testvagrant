let newsPapers = [
    {
        newspaperName : 'TOI',
        prices: [3,3,3,3,3,5,6]
    },
    {
        newspaperName : 'Hindu',
        prices: [2.5,2.5,2.5,2.5,2.5,4,4]
    },
    {
        newspaperName : 'ET',
        prices: [4, 4, 4, 4, 4, 4, 10]
    },
    {
        newspaperName : 'BM',
        prices: [1.5,1.5,1.5,1.5,1.5,1.5,1.5]
    },
    {
        newspaperName : 'HT',
        prices: [2, 2, 2, 2, 2, 4, 4]
    }
    ];
   
    const inputBudget = 35;
    let possibleCombinations = [];
   
    function getPossibleCombination() {
        newsPapers.forEach(e => {
            let total = 0;
            e.prices.forEach(el => {
                total = total + el;
            });
            e.total = total;
        });
        for(let i = 0 ; i < newsPapers.length - 1;i++){
            for(let j = i+1 ; j < newsPapers.length; j++){
                if(newsPapers[i].total + newsPapers[j].total <= inputBudget){
                    possibleCombinations.push([newsPapers[i].newspaperName, newsPapers[j].newspaperName])
                }
            }
        }
    }
    getPossibleCombination();
    console.log(possibleCombinations);
