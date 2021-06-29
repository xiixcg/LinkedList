var Node = (value) => {
  var node = {}

  node.value = value;
  node.next = null;

  return node;
}

class LinkedList {

  constructor() {
    var list = {}
    this.head = null;
    this.tail = null;
  }

  addToTail(value) {
    let currentNode = Node(value);
    if (this.head === null) {
      this.head = currentNode;
      this.list = { 'head': this.head }
    } else if (this.tail === null) {
      this.tail = currentNode;
      this.head.next = this.tail
    } else {
      let nextNode = this.head.next;
      while (nextNode.next !== null) {
        nextNode = nextNode.next;
      }
      nextNode.next = currentNode;
      this.tail = currentNode;
    }

  }

  removeHead() {
    let oldHead = this.head;
    this.head = this.head.next;
    return oldHead.value;
  }


let testLink = new LinkedList
testLink.addToTail(1)
testLink.addToTail(2)
testLink.addToTail(3)
testLink.addToTail(4)
console.log(testLink)
