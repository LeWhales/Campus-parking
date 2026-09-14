previous codes

function UserPermit(parkingzone, arrivalTime, accessibility, eventday) {
    (parkingzone = "Event", "Faculty", "General", "Student", "Visitor");
    (arrivalTime = "Normal hours", "After hours", "open any time");
    (accessibility = "no", "yes", "any");
    (eventday = "yes", "no");

}
function PolicyTable(parkingzone, arrivalTime, accessibility, allowed, eventday) {
    if ((parkingzone = "Faculty") && (arrivalTime = "normal hours") && (accessibility = "yes") && (allowed = "yes") && (eventday = "no")) console.log("Faculty permit during normal hours");
    else if ((parkingzone = "Faculty") && (arrivalTime = "after hours") && (accessibility = "yes") && (allowed = "yes") && (eventday = "no")) console.log("Faculty may use general parking after hours");
}

// case requirements
Case 	Permit 	Arrival Time 	Accessibility 	Event Day 	Allowed 	Zone 	Fee 	Reason
1 	Faculty 	Normal hours 	No 	            No 	            Yes 	Faculty     $0  Faculty permit during normal hours
2 	Faculty 	After hours 	No 	            No 	            Yes 	General 	$0 	Faculty may use general parking after hours
3 	Student 	Normal hours 	No 	            No 	            Yes 	Student 	$0 	Student permit during normal hours
4 	Student 	After hours 	No 	            No 	            Yes 	General 	$0 	Student may use general parking after hours
5 	Visitor 	Normal hours 	No 	            No 	            Yes 	Visitor 	$5 	Standard visitor parking fee
6 	Visitor 	After hours 	No 	            No 	            Yes 	General 	$3 	Reduced visitor fee after hours
7 	Visitor 	Any open time 	No 	            Yes 	        Yes 	Event 	$10 	Event-day visitor parking
8 	Any valid permit 	Any open time 	        Yes 	        No 	Yes 	Accessible 	$0 	Accessibility parking takes priority
9 	Any valid permit 	Any open time 	       Yes 	        Yes 	Yes 	Accessible 	$0 	Accessibility parking takes priority on event days
10 	Valid permit 	11 PM–5:59 AM 	Any 	Any 	No 	        None 	            $0 	Campus parking is closed


I can get it run but i am unsure how to get the remaining
