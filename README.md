Call this from wherever you want to increment the counter, use the provided html to show and clear the counter value.

function increaseCounter() {
    // Retrieve the counter from localStorage, default to 0 if not set
    let counter = parseInt(localStorage.getItem("genericCounter")) || 0;
    counter++; // Increase the counter
    localStorage.setItem("genericCounter", counter); // Save back to localStorage
    //return counter; // Return the updated counter if needed
}
