
Question 1
Let’s suppose you have the below JSX that gets returned from a component, what would be the equivalent object representation (Element) that React will create internally

 <button className='button-primary'>
    <div>
        Submit
    </div>
 </button>

 {
    type: "button",
    props: {
        className: "button-primary",
        children: {
            type: "div",
            props: {
                children: "Submit",
            } 
        },
    },
}
