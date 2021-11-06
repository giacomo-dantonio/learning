# Learning

Here I list the books I plan to read and some ideas for personal projects.

## Books

### Coding

Steve McConnell
    *Code Complete (second edition)*.

Andrew Hunt, David Thomas
    *The pragmatic programmer*.

Glenfold J. Myers
    *The Art of Software Testing*.

Robert C. Martin
    *Agile Software Development, Principles, Patterns, and Practices*.

Felienne Hermans
    *The Programmer's Brain*.

### Programming languages

Scott Meyers
    *Effective STL: 50 Specific Ways to Improve Your Use of the Standard Template Library*.

Scott Meyers
    *Effective Modern C++: 42 Specific Ways to Improve Your Use of C++11 and C++14*.

Luca Palmieri
    *Zero To Production In Rust*.

Jon Gjengset
    *Rust for Rustaceans. Idiomatic Programming for Experienced Developers*.

### Software architecture

Eric Evans
    *Domain-Driven Design: Tackling Complexity in the Heart of Software*.

Humberto Cervantes
    *Designing Software Architectures: A Practical Approach*.

Len Bass, Rick Kazman, Paul Clemens
    *Software Architecture in Practice*.

Gregor Hohpe and Bobby Woolf
    *Enterprise Integration Patterns*.

.NET application architecture documentation
    https://docs.microsoft.com/en-us/dotnet/architecture/

Thomas Erl
    *Service-Oriented Architecture, Second Edition*.

Paul Clemens, Felix Bachmann, Len Bass, David Garlan, James Ivers, ..
    *Documenting Software Architectures: Views and Beyond*.

Sam Newmann
    *Building microservices*.

Martin Fowler
    *Patterns of Enterprise Application Architecture*.

### Computer science

Harold Abelson, Gerald Jay Sussman
    *Structure and Interpretation of Computer Programs*.

Open Web Application Security Project (OWASP)
    https://www.owasp.org

Aho, Alfred Vaino; Lam, Monica Sin-Ling; Sethi, Ravi; Ullman, Jeffrey David
    *Compilers: Principles, Techniques, and Tools (2 ed.)*.

Stefan Höltgen
    *RESUME Hands-on Retrocomputing*.

### Machine Learning

Andriy Burkov
    *The Hundred-page Machine Learning Book*.

Andriy Burkov
    *Machine Learning Engineering*.

Aurélien Géron
    *Hands-on Machine Learning with Scikit-Learn, Keras and TensorFlow*.

### 3D and computational geometry

Les Piegl
    *The Nurbs Book*.

Jakob Andreas Bærentzen, Jens Gravesen, François Anton, Henrik Aanæs
    *Guide to Computational Geometry Processing*.

### Processes and management

Matthew Skelton
    *Team Topologies*.

Fred Brooks
    *The Mythical Man-Month: Essays on Software Engineering*.

### Mathematics

Jorge Nocedal, Stephen Wright
    *Numerical Optimization*.

William H. Press
    *Numerical Recipes: The Art of Scientific Computing*.

Gene H. Golub
    *Matrix Computations*.

Timothy A. Davis
    *Direct Methods for Sparse Linear Systems*.

Thomas R.J. Hughes
    *The Finite Element Method. Linear Static and Dynamic Finite Element Analysis*.

David Spiegelhalter
    *The Art of Statistics. Learning from Data*.

### Physics

Kip S. Thorne, Roger D. Blandford
    *Modern classical physics: Optics, Fluids, Plasmas, Elasticity, Relativity, and Statistical Physics*.

## Project ideas

### A user's manual for introverts in a tech job

This is a book, not a software project.
Recently I started researching the topic of how to be happy as an introvert
in a software job, without having to give up your goals and ambitions.
I collected some ideas and have some own ideas.

The next step is to write them down and share them with other.
While writing, I will probably have to do further and more detailed research.

I will write this using mdbook and upload it to github pages.

#### Status

Already started, but it will take some time.

### Photo manager

I have a lot of photos lying on a data storage in my home network.
They are accessible via smb. Since they are quite big, browsing through them
takes a long time and I struggle finding the photos, I am interested in.

This project consist of three parts. It is a web application which also uses
machine learning for picture classification.

The first part is a web application
which allows to browse to the folder structure of my photo storage.
The backend should resize the pictures to a smaller format and cache them
on the server side. It should provide endpoints for downloading
thumbnails and pictures in reduced size or in the original format.
The backend will resize and cache all the picture in one folder, as soon
one photo from that folder is requested. It should use an LRU caching strategy.

The second part will classify the photos with some tags (multiple labels
are possible), so that I can find things more quickly, without having to
browse through the folders. The web frondend needs to be able to assing
labels to the pictures. This should also be possible in batch (e.g. all the
picture in one folder get the same label). The labels needs to be persisted
on the backend. Finally it should be possible to search for all the pictures
with a given label. After a search, the server should only cache the search
results.

The third part is using machine learning to automatically classify new photos.
An model will be trained with the labels manually entered
by the user. When new pictures are added to the storage, the application
will automatically assign labels to the new files. The user should be able
to remove or add some labels (also in batch) and retrain the model.

#### Status

Not started yet.

### Personal page and CV

### Tides prediction

### Non violent communication

### Marathon passing times