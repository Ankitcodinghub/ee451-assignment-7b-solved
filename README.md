# ee451-assignment-7b-solved
**TO GET THIS SOLUTION VISIT:** [EE451 Assignment 7b Solved](https://www.ankitcodinghub.com/product/ee451-assignment-7b-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;100485&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;EE451 Assignment 7b Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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

<div class="kksr-stars-active" style="width: 0px;">
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
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
1. Examples

The hello.cu contains the CUDA implementation of HelloWorld.

<ol>
<li>Login to HPC</li>
<li>Setup MPI toolchain:</li>
<li>Compile
nvcc -O3 -arch=sm_20 hello.cu
</li>
<li>Run
The option -t specifies the limit of run time. Setting it as a small number will get your program scheduled earlier. For more information on srun options, you can use man srun to find out.
</li>
<li>Profile (optional)
srun -n1 –gres=gpu:p100:1 –partition=debug nvprof ./a.out
</li>
<li>Allocate a machine</li>
</ol>
</div>
</div>
<div class="layoutArea">
<div class="column">
module purge

module load gcc /8.3.0 cuda /10.1.243

</div>
</div>
<div class="layoutArea">
<div class="column">
srun -n1 –gres=gpu:1 -t1 ./a.out

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
salloc -n1 –gres=gpu:1 –mem=16G -t10

// After the allocation, you will log on the machine and have 10 minutes to perform multiple operations

./a.out

// edit , compile , and run again without waiting for a new allocation

./a.out ./a.out

</div>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
2. (100 points) 1024 × 1024 matrix multiplication using these two approaches. • Approach 1 (unoptimized implementation using global memory only) :

– Name this program as ‘mm1.cu’

– The value of each element of A is 1

– The value of each element of B is 2

– Thread block configuration: 16 × 16

– Grid configuration: 64 × 64

– After computation, print the value of C[451][451]

• Approach 2 (block matrix multiplication using shared memory) :

<ul>
<li>– &nbsp;Name this program as ‘mm2.cu’</li>
<li>– &nbsp;The value of each element of A is 1</li>
<li>– &nbsp;The value of each element of B is 2</li>
<li>– &nbsp;Thread block configuration: 32 × 32</li>
<li>– &nbsp;Grid configuration: 32 × 32</li>
<li>– &nbsp;More details of this algorithm can be found in the paper ‘Matrix Multiplication with CUDA’.</li>
<li>– &nbsp;After computation, print the value of C[451][451]

Measure the execution time of the kernel of Approach 1 and Approach 2, respectively.

Submission Instructions: Submit your code, screenshots, and a performance report as described above.
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column"></div>
</div>
<div class="layoutArea"></div>
</div>
