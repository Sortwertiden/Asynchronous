# Asynchronous
Asynchronous JavaScript with Async/Await
function resolveAfter2Seconds() {
    return new Promise(resolve => {
        setTimeout(() => {
            resolve('Resolved after 2 seconds');
        }, 2000);
    });
}

async function asyncCall() {
    console.log('Calling async function');
    const result = await resolveAfter2Seconds();
    console.log(result);
}

asyncCall();
