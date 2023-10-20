# SQL
Using an interface with c#. Iterfaces take advantage of inheritance. It works as a template of what a class needs to have.


This is what the interface piblic class would look like

public interface IRepository<T, Tid>;
{
    List<T> Get();

    T GetById(Tid id);

    T Create(T newData)

public int Update(T updateDate);

public int Delte(tid id);
{
}
}

then we would call this in whatever repostory we want to put it in.
This is how we call on the interface in the repo.

public class NameOfRepository :
Irepository<NameOfRepository, int>
