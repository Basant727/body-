function calculateBMI() {
    const weight = parseFloat(document.getElementById('weight').value);
    const height = parseFloat(document.getElementById('height').value);
    const result = document.getElementById('result');
    const advice = document.getElementById('advice');

    if (weight > 0 && height > 0) {
        const bmi = weight / (height * height);
        result.innerHTML = `Your BMI is ${bmi.toFixed(2)}`;

        if (bmi > 20) {
            const weightToLose = weight - (20 * height * height);

            advice.innerHTML = `
                <p>To reach a BMI of 20, you need to lose approximately ${weightToLose.toFixed(2)} kg.</p>
                <p>Choose any one of the activity to follow:</p>
                <ul>
                    <li><strong>Run:</strong> ${((weightToLose * 77) / 1350).toFixed(2)} hours daily for 6 months.</li>
                    <li><strong>Cycle:</strong> ${((weightToLose * 231) / 2700).toFixed(2)} hours daily for 6 months.</li>
                    <li><strong>Walk:</strong> ${((weightToLose * 231) / 1350).toFixed(2)} hours daily for 6 months.</li>
                    <li><strong>Walk:</strong> ${((weightToLose * 231*6250) / 1350).toFixed(2)} steps daily for 6 months.</li>
                    
                </ul>
                <p>Stay consistent and you'll be fit soon!</p>
                <p>note thing are calculated as an approximate result  </p>
                <p>© basantsaini</p>
            `;
        } else {
            advice.innerHTML = `<p>Your BMI is already healthy! Keep up the good work!</p>`;
        }
    } else {
        alert("Please enter valid weight and height.");
    }
}

