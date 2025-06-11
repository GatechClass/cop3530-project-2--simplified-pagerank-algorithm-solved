# cop3530-project-2--simplified-pagerank-algorithm-solved
**TO GET THIS SOLUTION VISIT:** [COP3530 Project 2- Simplified PageRank Algorithm Solved](https://mantutor.com/product/cop3530-simplified-pagerank-algorithm-solved/)


---

**For Custom/Order Solutions:** **Email:** mantutorcodes@gmail.com  

*We deliver quick, professional, and affordable assignment help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;97388&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;6&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (6 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COP3530 Project 2- Simplified PageRank Algorithm Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (6 votes)    </div>
    </div>
In late 90’s as the number of webpages on the internet was growing exponentially different search engines were trying different approaches to rank the webpages. At Stanford, two computer science Ph.D. students, Sergey Brin and Larry Page were working on the following questions: How can we trust information? Why are some web pages more important than others? Their research led to the formation of the Google search engine.

In this project, you are required to implement a simplified version of the original PageRank algorithm on which Google was built by representing the web as a graph and implementing this graph using an Adjacency List or an equivalent data structure. The PageRank algorithm is an algorithm that is used to order or rank different web pages on the internet.

Representing the Web as a Graph

The entire internet consists of different webpages that can be represented as a graph. Each node represents a webpage and each edge represents a link between two webpages. This graph can be implemented as an Adjacency Matrix or an Adjacency List. In this assignment, you are supposed to implement the Adjacency List representation. If you use an Adjacency Matrix representation, you will be penalized by 50% of your implementation points and will also fail the large test cases.

Adjacency Matrix Representation

Now for the sake of simplicity, we are explaining the project in the form of an Adjacency Matrix, M. We represent the internet in the form of |V|x|V| matrix where |V| is the total number of vertices in this graph or the total number of webpages in the internet. Each vertex, Vi is a webpage in the entire internet. In the below graph, we have five vertices or webpages. Within our graph, if there is an edge from Vi to Vj (the from_page points to_page), we have the value in our adjacency matrix Mij = 1 and 0 otherwise.

1

2

3 0 1 0 1 0

0 0 0 1 0

0 0 0 0 1

4

5 0 0 1 0 0

1 1 0 0 0

1 2 3 4 5

M=

Each webpage is thus a node in the directed graph and has incoming edges and outgoing edges. Each node has a rank, r. According to PageRank, this rank, r is equally split among the node’s outgoing links. In the below figure, rank of node i, is denoted by ir and this rank is equally split among node i’s three outgoing edges.

Rank(i) = Rank(j)/out_degree(j) + Rank(k)/out_degree(k)

According to PageRank, this rank, r is equal to the sum of the incoming ranks. In the above figure, rank of node i, ir = kr/out_degree(k) + jr/out_degree(j); Thus, the rank is based on the indegree (the number of nodes pointing to it) and the importance of an incoming node. This is important considering let’s say you create your personal website and have a million links to other pages of importance, then you might artificially inflate your website’s ranking if this was not the case. If for calculating the rank, we used out links, we could have easily duped the algorithm. Therefore, the rank is only based on in-links.

1 0 1 0 1 0

2

3 0 0 0 1 0

0 0 0 0 1

4 0 0 1 0 0

5 1 1 0 0 0

1 2 3 4 5

M=

Core Idea of PageRank

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> Important web pages will point to other important webpages.

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> Each page will have a score and the results of the search will be based on the page score (called page rank).

Goal

In this assignment, you need to compute the rank of the webpages using a Simplified PageRank Algorithm explained in the example below. You are supposed to implement an Adjacency List data structure to represent the graph.

Input

Line 1 contains the number of lines (n) that will follow and the number of power iterations (p) you need to perform. Each line from 2 to n+1 will contain two URL’s – from_page to_page separated by a single space. This means that the from_page points to the URL to_page.

Output

Print the PageRank of all pages after p powerIterations in ascending alphabetical order of webpage. Also, round off the rank of the page to two decimal places.

Constraints

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> 1 &lt;= p &lt;= 10,000

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> 1 &lt;= n &lt;= 10,000

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> 1 &lt;= Unique webpages or |V| &lt;= 10000

Explanation of PageRank through an Adjacency Matrix Example

Gradescope Test Case 1 Explanation (p=2):

Input

7 2 google.com google.com facebook.com ufl.edu ufl.edu maps.com gmail.com gmail.com maps.com

ufl.edu google.com gmail.com facebook.com maps.com Output

facebook.com 0.20 gmail.com 0.20 google.com 0.10 maps.com 0.30 ufl.edu 0.20

Note: Here, p = 2, n = 7, |V| = 5

Graph Representation of Above Input

1 google.com

2

3

4

5 gmail.com

facebook.com

maps.com

ufl.edu

Data Structure 1

Algorithm

Step 1: Mapping for Simplicity (Optional but you will need a mechanism to store unique vertices) Use a map/associative array to map the URL’s with a unique id

1 google.com

2 gmail.com

3 facebook.com

4 maps.com

5 ufl.edu

Step 2: Graph Representation and Page Rank

In PageRank, the equation to calculate the rank for your graph is given as follows:

Rank of a Page, r = M.r where,

M is the matrix with values given by the following:

Mij = 1/dj if there is an edge from Vj to Vi (dj is the outdegree of node j) 0 otherwise

For our graph, the adjacency matrix, M will look like: 1 2 3 4 5

1 0 0 0 0 1/d5

2

3 1/d1 0 0 0 1/d5

0 0 0 1/d4 0

4 1/d1 1/d2 0 0 0

5 0 0 1/d3 0 0

Step 3: Power iteration, r(t+1) = M.r(t)

This means that a rank of the webpage at time t+1 is equal to the rank of that page at time t multiplied by matrix, M. To achieve this, we create our matrix M based on input. Next, we initialize r(t) which is a matrix of size |V|x1 and consists of the ranks of every webpage. We initialize r(t) to 1/|V|. Next, we compute power_iterations based on our input, p. There is a mathematical proof that the matrix r converges, i.e. r(t+1) = r(t) at which point the algorithm stops. However, this is difficult to test and we therefore will be testing your algorithm on a fixed power iteration value, p.

Example r and M matrices for our input:

r(0) M

1 1 2 3 4 5

1 1/5

2

3 1/5

1/5

4 1/5

5 1/5

1

2 0 0 0 0 1/d5

1/d1 0 0 0 1/d5

3 0 0 0 1/d4 0

4 1/d1 1/d2 0 0 0

5 0 0 1/d3 0 0

1 2 3 4 5 1 1

1

1

2

3

4

5 1/10

1/5

1/5

3/10

1/5

0 0 0 0 1/2 1

2 1/5

1/2 0 0 0 1/2 1/5

0 0 0 1 0 x 3

4

5 1/5

1/2 1 0 0 0 1/5

0 0 1 0 0 1/5

r(1) = M.r(0) = 2 =

3

4

5

M x r(0) = r(1)

Note: In our input case, the number of power_iterations, p is 2. Therefore we print r(1) of the urls sorting in alphabetical order. If p was 1 then return the initializing rank matrix or r(0). If p&gt;2, the process repeats where you multiply the matrix, M with the new rank matrix r(t+1) at the next iteration.

Gradescope Test Case 2 Explanation (p=3):

1 2 3 4 5 1 1

1

1

2

3

4

5 1/10

3/20

3/10

1/4

1/5

0 0 0 0 1/2 1 1/10

1/2 0 0 0 1/2 2 1/5

0 0 0 1 0 x 3 1/5

1/2 1 0 0 0 4

5 3/10

0 0 1 0 0 1/5

r(t+1) = r(2) = M.r(1) = 2 =

3

4

5

M x r(1) = r(2)

Optional Template

You are allowed to use your own template but make sure your code passes the sample test cases. An example template to think about the problem is:

class AdjacencyList { private:

//Think about what member variables you need to initialize public:

//Think about what helper functions you will need in the algorithm

};

void AdjacencyList::PageRank(int n){ } // prints the PageRank of all pages after p powerIterations in ascending alphabetical order of webpages and rounding rank to two decimal places

// This class and method are optional. To accept the input, you can use this method:

int main()

{ int no_of_lines, power_iterations;

std::string from, to; std::cin &gt;&gt; no_of_lines; std::cin &gt;&gt; power_iterations;

for(int i = 0;I &lt; no_of_lines; i++)

{ std::cin &gt;&gt; from; std::cin &gt;&gt; to; // Do Something

}

//Create a graph object

Created_Graph.PageRank(power_iterations);

}

Testing

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> Test your code on Gradescope before submitting your implementation. You have five available test cases and you can submit any number of times.

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> Create your own tests and test as much as possible. Our recommendation is you spend at least 1-2 hours on testing extensively.

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> We will stick to the input format. No need to test for off-input statement such as inputting one url instead of two in a line or testing whether a url is valid or not.

Grading

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> Implementation [75 points] o You are supposed to implement an Adjacency List data structure to represent the graph. Failure to implement this will incur a 25 points deduction.

o Your code will be tested on 15 test cases each worth 5 points:

• 5 publicly available test cases.

• 10 test cases that will be added by the course staff and are not shown to the students.

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> Documentation [15 Points] o Submit a document addressing all these prompts:

• Describe the data structure you used to implement the graph and why? [2.5 points]

• What is the computational complexity of each method in your implementation in the worst case in terms of Big O notation? [5 points]

• What is the computational complexity of your main method in your implementation in the worst case in terms of Big O notation? [5 points]

• What did you learn from this assignment and what would you do differently if you had to start over?

[2.5 points]

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> Code Style and Design [10 Points] o 5 points for design decisions, a well-designed Graph API, and code modularity o 2 points for appropriate comments o 1 point for white spaces

o 2 points for consistent naming conventions

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> Catch Tests Bonus [5 Points] o You can score 5 bonus points if you submit a separate file containing 5 test cases (1 point/test) using the Catch Framework. These tests should be different than the public test cases. Your score is however capped to 100 points for this project. This means that if you pass 14 tests and submit bonus test files, you will get a 100 provided you score full points on the documentation. Also, if you pass 15 tests and score 23 on documentation and design, + 5 points on bonus, you will still score 100 points [your score is 103 but is capped to 100 in this case].

Submission

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> One or more .cpp or.h files that have your implementation. Test on gradescope early and often.

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> One pdf file that has your documentation. Upper limit – 3 pages with 20% deduction in report per extra page. Cover page is not required, just your name on Page 1 is suffice.

Frequently Asked Questions

Based on the number of repeated questions we got in Project 1 on Slack, the course staff will now maintain an active FAQ Google document to answer your questions. Post your questions in Slack, but this time we will answer in this document and send you the link. The link to the document is:

https://docs.google.com/document/d/1a9hR1Ep2IYK-MnsXwl2VxyotO1Yd-XCC8NWUkdp24JM/

Additional Optional Resources

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> Page Rank Paper: http://ilpubs.stanford.edu:8090/422/1/1999-66.pdf

<img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> Videos on Page Rank (The assignment is based on these videos): Lectures 5-8 <img draggable="false" role="img" class="emoji" alt="▪" src="https://s.w.org/images/core/emoji/15.1.0/svg/25aa.svg"> Extended Videos (Not required for Project): Lecture 9-11
